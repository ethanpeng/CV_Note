### OSVR CV Kalman Trace 流程

OSVR-Core/plugins/videobasedtracker/BeaconBasedPoseEstimator_Kalman.cpp  
[kalman::correct(state, model, meas);](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/plugins/videobasedtracker/BeaconBasedPoseEstimator_Kalman.cpp#L247) 
↓  
OSVR-Core/inc/osvr/Kalman/FlexibleKalmanFilter.h  
[correct()](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/inc/osvr/Kalman/FlexibleKalmanFilter.h#L58)  
↓  
OSVR-Core/inc/osvr/Kalman/FlexibleKalmanCorrect.h  
[beginCorrection()](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/inc/osvr/Kalman/FlexibleKalmanCorrect.h#L135) {  
...  
[S = H * PHt + R;](https://github.com/ethanpeng/OSVR-Core/blob/59405fc1b1a25aea051dfbba0be5171fa19b8b30/inc/osvr/Kalman/FlexibleKalmanCorrect.h#L157)  
}  

