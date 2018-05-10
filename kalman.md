### OSVR CV Kalman Trace 流程

[OSVR-Core\plugins\videobasedtracker\VideoBasedTracker.cpp](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/plugins/videobasedtracker/VideoBasedTracker.cpp)  
VideoBasedTracker::processImage() {  
[m_estimators[sensor]->EstimatePoseFromLeds()](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/plugins/videobasedtracker/VideoBasedTracker.cpp#L202)  
}  

[OSVR-Core\plugins\videobasedtracker\BeaconBasedPoseEstimator.cpp](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/plugins/videobasedtracker/BeaconBasedPoseEstimator.cpp)  
BeaconBasedPoseEstimator::EstimatePoseFromLeds() {  
	m_estimatePoseFromLeds()  
}  
↓  
BeaconBasedPoseEstimator::m_estimatePoseFromLeds() {  
	...  
	if (!m_gotPose || !m_gotPrev || !m_permitKalman) {  
	result = m_pnpransacEstimator(leds);  
	} else {  
	result = m_kalmanAutocalibEstimator(leds, dt); // 用 kalman →  
	...  
	// 取出 state 再送 pose 出去  
}  

OSVR-Core/plugins/videobasedtracker/BeaconBasedPoseEstimator_Kalman.cpp  
[BeaconBasedPoseEstimator::m_kalmanAutocalibEstimator()](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/plugins/videobasedtracker/BeaconBasedPoseEstimator_Kalman.cpp#L61) {  
	[kalman::predict(m_state, m_model, dt);](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/plugins/videobasedtracker/BeaconBasedPoseEstimator_Kalman.cpp#L135)  // 預測  
	...  
	[kalman::correct(state, model, meas);](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/plugins/videobasedtracker/BeaconBasedPoseEstimator_Kalman.cpp#L247) // 修正 →  
}  
↓  
OSVR-Core/inc/osvr/Kalman/FlexibleKalmanFilter.h  
[correct()](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/inc/osvr/Kalman/FlexibleKalmanFilter.h#L58)  
↓  
OSVR-Core/inc/osvr/Kalman/FlexibleKalmanCorrect.h  
[beginCorrection()](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/inc/osvr/Kalman/FlexibleKalmanCorrect.h#L135) {  
...  
[S = H * PHt + R;](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/inc/osvr/Kalman/FlexibleKalmanCorrect.h#L157)  
}  

