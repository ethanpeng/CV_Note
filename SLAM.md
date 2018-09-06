# SLAM
### 1. 導論
#### 視覺SLAM十四講
[【SLAM】视觉SLAM高博十四讲 影片](https://www.bilibili.com/video/av19397094/)  
[視覺slam十四講總結PPT](https://download.csdn.net/download/sinat_16615673/10493814?utm_source=bbsseo)  
[gaoxiang12/slambook](https://github.com/gaoxiang12/slambook)  
[書本目錄](https://www.tenlong.com.tw/products/9787121311048)  

ch4  
旋轉矩陣有約束（正交且行列式為1）,使得優化變得困難  
李代數可以變成無約束優化  

特殊正交群SO(3)

so(3) 3x3矩陣  
se(3) 4x4矩陣  



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

[UCF Computer Vision 課程簡介](http://crcv.ucf.edu/courses/CAP5415/Fall2014/index.php)  
[UCF Computer Vision](https://www.youtube.com/playlist?list=PLd3hlSJsX_ImKP68wfKZJVIPTd8Ie5u-9)  
L4 看了一些  
[UCF Computer Vision Video Lectures 2014 (部分中英字幕）](https://www.bilibili.com/video/av29974804/)  

[泡泡机器人 - TA的视频](https://space.bilibili.com/38737757/#/)  
[github.io - 圖像視覺："行人檢測任務之FHOG算子"](http://cwlseu.github.io/Feature-descriptor-fhog/)
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

### 3D track viewer
[ORB-SLAM2: an Open-Source SLAM for Monocular, Stereo and RGB-D Cameras](https://www.youtube.com/watch?v=ufvPS5wJAx0) - Pangolin   
[ROS - rviz](https://blog.csdn.net/github_35160620/article/details/52513334)  
[OpenCV sfm - Camera Motion Estimation](https://docs.opencv.org/3.1.0/d5/dab/tutorial_sfm_trajectory_estimation.html)  
[OpenCV sfm - Scene Reconstruction](https://docs.opencv.org/3.1.0/d4/d18/tutorial_sfm_scene_reconstruction.html)  

## 2D Wave
QT - Qwt  

### KCF
[作者的首頁](http://www.robots.ox.ac.uk/~joao/circulant/)  
[KCF跟踪源码-带注释](https://blog.csdn.net/jacke121/article/details/54315050)  
[目標跟蹤算法——KCF入門詳解](https://blog.csdn.net/crazyice521/article/details/53525366)
[【目標跟蹤】KCF高速跟蹤詳解](https://blog.csdn.net/shenxiaolu1984/article/details/50905283)  
[目標跟蹤：KCF](https://lidongxuan.github.io/blog/kcf)  
[核化相关滤波器高速跟踪：KCF(2015PAMI)](https://zhuanlan.zhihu.com/p/26685032)  
[KCF目标跟踪算法](https://www.jianshu.com/p/9aacd075a689)  
[KCF目標跟蹤方法分析與總結](https://www.cnblogs.com/YiXiaoZhou/p/5925019.html)
[Kernelized Correlation Filters (KCF) Tracking算法](https://blog.csdn.net/wanghanthu/article/details/53375393)  
[Introduction to OpenCV Tracker](https://docs.opencv.org/3.1.0/d2/d0a/tutorial_introduction_to_tracker.html)  
[目标跟踪：KCF运行流程图(matlab版本)](https://blog.csdn.net/JasonSunJian/article/details/71489097)  

### 傅立葉轉換
[阿洲的程式教學 - 傅立葉轉換(Fourier Transform)](http://monkeycoding.com/?p=864)  
[如果看了此文你還不懂傅里葉變換(Fourier+Transform)，那就過來掐死我吧!](http://blog.xuite.net/lapuda.chen/PaulBlog/221866406-%E5%A6%82%E6%9E%9C%E7%9C%8B%E4%BA%86%E6%AD%A4%E6%96%87%E4%BD%A0%E9%82%84%E4%B8%8D%E6%87%82%E5%82%85%E9%87%8C%E8%91%89%E8%AE%8A%E6%8F%9B%28Fourier+Transform%29%EF%BC%8C%E9%82%A3%E5%B0%B1%E9%81%8E%E4%BE%86%E6%8E%90%E6%AD%BB%E6%88%91%E5%90%A7%21)  
[傅里葉分析之掐死教程（完整版）更新於2014.06.06](https://zhuanlan.zhihu.com/p/19763358)  
[傅里叶分析之掐死教程](https://daily.zhihu.com/story/3955477)  
[Wave](http://www.csie.ntnu.edu.tw/~u91029/Wave.html)  
[[OpenCV-Python] OpenCV 中的影象處理 部分 IV (六)](https://tw.saowen.com/a/bd88bee600238de9086b325dcdf7039a5c99ed622331b3a54bcbdb7a36013f76)  
[Python下opencv使用笔记（十）（图像频域滤波与傅里叶变换）](https://blog.csdn.net/on2way/article/details/46981825)  
