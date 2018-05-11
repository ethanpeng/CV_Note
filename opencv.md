# opencv

fix  
[mergeLabels()](https://github.com/opencv/opencv/blob/000a13b6a35f65eb04e5c78721364406718f5d81/modules/imgproc/src/connectedcomponents.cpp#L2469)  
[mergeLabels8Connectivity()](https://github.com/opencv/opencv/blob/000a13b6a35f65eb04e5c78721364406718f5d81/modules/imgproc/src/connectedcomponents.cpp#L500)  

Spell Checker github


### issues
Memory leak in GaussianBlur  
https://github.com/opencv/opencv/issues/11449  



### [ubuntu下opencv2.4.9和opencv3.1.0的使用](https://blog.csdn.net/qq_30356613/article/details/70339731)  

build and install opencv-3.1.0  
```
cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local/opencv-3.1.0 ..
make
sudo make install
```

build and install opencv-2.4.9  
```
cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local/opencv-2.4.9 ..
make
sudo make install
```

用 opencv3.1.0, CMakeLists.txt  
```
cmake_minimum_required(VERSION 2.8)
set(OpenCV_DIR "/usr/local/opencv-3.1.0/share/OpenCV")
#include_directories("/usr/local/opencv-3.1.0/include")
project(test)
find_package(OpenCV 3.1.0 REQUIRED)
add_executable(test test.cpp)
include_directories(${OpenCV_INCLUDE_DIRS})
target_link_libraries(test ${OpenCV_LIBS})  
```
用 opencv2.4.9, CMakeLists.txt  
```
cmake_minimum_required(VERSION 2.8)
set(OpenCV_DIR "/usr/local/opencv-2.4.9/share/OpenCV")
#include_directories("/usr/local/opencv-2.4.9/include")
project(test)
find_package(OpenCV 2.4.9 REQUIRED)
add_executable(test test.cpp)
include_directories(${OpenCV_INCLUDE_DIRS})
target_link_libraries(test ${OpenCV_LIBS})
```
