# Obstacle Detection using LiDAR

Implemented a Obstacle Detection pipeline using LiDAR Point Cloud segmentation, 3D RANSAC, KD-Tree and Euclidean clustering algorithm.

<img src="media/obstacle-detection-fps-final.gif" width="800" height="400" />

<br/>
<br/>

### Files
* ```src```
    * ```render```
        * ```box.h```: Defines the structure of the box objects.
        * ```render.h```, ```render.cpp```: Defines classes and methods for rendering objects.
    * ```sensors```
        * ```lidar.h```: Functions using ray casting for creating PCD
    * ```environment.cpp```: main file for using PCL viewer and processing/visualizing PCD
    * ```processPointClouds.h```, ```processPointClouds.cpp```: Functions for filtering, segmenting, clustering, boxing, loading and saving PCD

<br/>
<br/>

### Important Dependencies
* Ubuntu 16.04
* PCL - v1.7.2
* C++ v11
* gcc v5.5

<br/>

### Build Instructions
```
cd ~/Obstacle-Detection-using-LiDAR
mkdir build && cd build
cmake ..
make
./environment
```