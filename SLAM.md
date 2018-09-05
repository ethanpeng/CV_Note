# SLAM
### 1. 導論
#### 視覺SLAM十四講
[【SLAM】视觉SLAM高博十四讲 影片](https://www.bilibili.com/video/av19397094/)  
[書本目錄](https://www.tenlong.com.tw/products/9787121311048)  

ch4  
旋轉矩陣有約束（正交且行列式為1）,使得優化變得困難  
李代數可以變成無約束優化  

特殊正交群SO(3)


#### 文章
[Visual SLAM算法筆記](https://blog.csdn.net/mulinb/article/details/53421864)  
[三維重建6：綁架問題/SensorFusion/IMU+CV-小尺度SLAM](https://blog.csdn.net/wishchin/article/details/73484680)  
蒙特卡洛估計器，即粒子濾波方法  
[三維重建7：Visual SLAM算法筆記](https://blog.csdn.net/wishchin/article/details/73511679)  
[vio 入門概念](https://blog.csdn.net/datase/article/details/78682156)  
[視覺慣性里程計Visual–Inertial Odometry(VIO)概述](https://www.cnblogs.com/hitcm/p/6327442.html)  
filter-based  
緊耦合: 比較經典的算法是MSCKF，ROVIO  
松耦合: [ssf](https://github.com/ethz-asl/ethzasl_sensor_fusion)  
optimization-based  


### LSD SLAM
[tum-vision/lsd_slam](https://github.com/tum-vision/lsd_slam)  
[深入學習 LSD-SLAM – 1](https://blog.techbridge.cc/2017/03/18/lsd-slam-1/)  


### ORB SLAM
[raulmur/ORB_SLAM2](https://github.com/raulmur/ORB_SLAM2) - Real-Time SLAM for Monocular, Stereo and RGB-D Cameras, with Loop Detection and Relocalization Capabilities  

### DSO
[JakobEngel/dso](https://github.com/JakobEngel/dso) - Direct Sparse Odometry  
[DSO: Direct Sparse Odometry 官網](https://vision.in.tum.de/research/vslam/dso?redirect=1)  
[DSO: Direct Sparse Odometry](https://www.youtube.com/watch?v=C6-xwSOOdqQ)  

### 部落格與文章
[DSO代碼閱讀](https://x007dwd.github.io/2017/02/28/dso-slam/)  
[DSO 初探](https://blog.csdn.net/heyijia0327/article/details/53173146)  

### 討論
[知乎 orb-slam在眾多SLAM方法中處於怎樣的地位？](https://www.zhihu.com/question/35116055) - 作者個人的一些看法, 附上kinect2上的視頻.  
[ORB-SLAM vs. DSO: Possible to develop DSO to the same level?]() - 提到  it seems to be that ORB-SLAM(2) and DSO seem to be the two currently best (openly available) algorithms.

