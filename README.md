# jetson_ros_docker

## Introduction
This is a Dockerfile to launch ROS on NVIDIA Jetson devices.  
And, this project has the following Dockerfile.

- [master](https://github.com/atinfinity/jetson_ros_docker/tree/master)
  - This Dockerfile uses [nvcr.io/nvidia/l4t-base](https://ngc.nvidia.com/catalog/containers/nvidia:l4t-base) as base Docker image.
  - ROS Distribution: [ROS Melodic Morenia](http://wiki.ros.org/melodic)
- [melodic](https://github.com/atinfinity/jetson_ros_docker/tree/melodic)
  - This Dockerfile uses [arm64v8/ubuntu:18.04](https://hub.docker.com/r/arm64v8/ubuntu/) as base Docker image.
  - ROS Distribution: [ROS Melodic Morenia](http://wiki.ros.org/melodic)
- [kinetic](https://github.com/atinfinity/jetson_ros_docker/tree/kinetic)
  - This Dockerfile uses [arm64v8/ubuntu:16.04](https://hub.docker.com/r/arm64v8/ubuntu/) as base Docker image.
  - ROS Distribution: [ROS Kinetic Kame](http://wiki.ros.org/kinetic)

## Requirements
- Docker

## Preparation
### Build Docker image
```
$ docker build -t jetson/ros:kinetic .
```

### Create Docker container
```
$ ./launch_container.sh
```

## Launch roscore
```
$ roscore
```
