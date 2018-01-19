# Introduction

This is a fork of peac (http://www.merl.com/research/license). Details in /include/README.md
PEAC(Plane Extraction using Agglomerative Clustering) is a fast plane segmentation algorithm for **organized** point cloud. Frame rate can be
more than 35Hz for 640×480 point clouds.

> Feng C, Taguchi Y, Kamat V R. Fast plane extraction in organized point clouds using agglomerative hierarchical clustering[C]// IEEE International Conference on Robotics and Automation. IEEE, 2014:6218-6225.

This fork:
- add demo code which use opencv only(no pcl) to show how to run
- provice raw code and paper

Node:
- PEAC only support organized point cloud which can be generated from depth image or disparity image.
- PEAC code has only headers, so it can be easily integrated into your projects.
- PEAC assumes mm as unit. So input cloud should be in mm unit, or the algorithm param inside maybe invalid.

# Prerequisites

Prerequisites needed for compiling PEAC using c++:
- OpenCV (http://opencv.org)

# How to run

```
mkdir build
cd build
cmake ..
make
./demo_peac
```
