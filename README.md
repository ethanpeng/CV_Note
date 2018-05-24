# pnp

[solvePnP flags](https://github.com/opencv/opencv/blob/10ba6a93a6fee952fb7812b28989eb209d4f49a1/modules/calib3d/include/opencv2/calib3d.hpp#L235)
```
enum { SOLVEPNP_ITERATIVE = 0,
       SOLVEPNP_EPNP      = 1, //!< EPnP: Efficient Perspective-n-Point Camera Pose Estimation @cite lepetit2009epnp
       SOLVEPNP_P3P       = 2, //!< Complete Solution Classification for the Perspective-Three-Point Problem @cite gao2003complete
       SOLVEPNP_DLS       = 3, //!< A Direct Least-Squares (DLS) Method for PnP  @cite hesch2011direct
       SOLVEPNP_UPNP      = 4, //!< Exhaustive Linearization for Robust Camera Pose and Focal Length Estimation @cite penate2013exhaustive
       SOLVEPNP_AP3P      = 5, //!< An Efficient Algebraic Solution to the Perspective-Three-Point Problem @cite Ke17
       SOLVEPNP_MAX_COUNT      //!< Used for count
};
```

[solvePnP()](https://github.com/opencv/opencv/blob/7dc88f26f24fa3fd564a282b2438c3ac0263cd2f/modules/calib3d/src/solvepnp.cpp#L56)  - opencv/modules/calib3d/src/solvepnp.cpp  
```
bool solvePnP( InputArray _opoints, InputArray _ipoints,
               InputArray _cameraMatrix, InputArray _distCoeffs,
               OutputArray _rvec, OutputArray _tvec, bool useExtrinsicGuess, int flags )
{ ...
```

[cvFindExtrinsicCameraParams2()](https://github.com/opencv/opencv/blob/e268fdc0ed89be11ce2e6d7a8832254fc4b67ccc/modules/calib3d/src/calibration.cpp#L969) - opencv/modules/calib3d/src/calibration.cpp  
```
CV_IMPL void cvFindExtrinsicCameraParams2( const CvMat* objectPoints,
                  const CvMat* imagePoints, const CvMat* A,
                  const CvMat* distCoeffs, CvMat* rvec, CvMat* tvec,
                  int useExtrinsicGuess )
```

[findHomography()](https://github.com/opencv/opencv/blob/e268fdc0ed89be11ce2e6d7a8832254fc4b67ccc/modules/calib3d/src/fundam.cpp#L350) - opencv/modules/calib3d/src/fundam.cpp  
```
cv::Mat cv::findHomography( InputArray _points1, InputArray _points2,
                            int method, double ransacReprojThreshold, OutputArray _mask,
                            const int maxIters, const double confidence)
```
method: 最小中值法、RANSAC方法、最小二乘法 [ref](https://blog.csdn.net/luoshixian099/article/details/50217655)   

[urbste/MLPnP_matlab_toolbox](https://github.com/urbste/MLPnP_matlab_toolbox) - The toolbox is a collection of PnP methods for Matlab. 有時間試試 
