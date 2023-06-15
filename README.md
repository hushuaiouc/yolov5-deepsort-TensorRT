Yolov5 and Deepsort TenoorRT in Jetson Xavier nx and Jetson nano


This repository uses yolov5 and deepsort to track human which can run in Jetson Xavier nx and Jetson nano. 


For more details, please refer to [BILIBILI](). We recorded a detailed video on how to run this project.

## Requirement
1. Jetson nano or Jetson Xavier nx
2. Jetpack 4.6.1



if you have problem in this project, please pull a issue.

## Environment

```shell
git clone --recursive https://github.com/dusty-nv/jetson-inference
docker pull dustynv/jetson-inference:r32.7.1
cd jetson-inference
docker/run.sh
```
 more details see the [BILIBILI]()


## Build and Run

```shell
git clone 
cd yolov5-deepsort-tensorrt
// before you cmake and make, please change ./src/main.cpp char* yolo_engine = ""; char* sort_engine = ""; to your own path
mkdir build
cd build 
cmake ..
make 
```

## References
1.https://github.com/RichardoMrMu/yolov5-deepsort-tensorrt

2.https://github.com/dusty-nv/jetson-inference
