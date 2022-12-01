# Usage Instructions

## Start up the ROS Master Node

```roscore```

## Setup connection with the robot

```sudo chmod +777 /dev/ttyUSB0```

```rosrun rosaria RosAria```

## Setting up the Camera

```roslaunch realsense2_camera rs_camera.launch align_depth:=true```

To get pointclouds from the RGBD images:

```roslaunch realsense2_camera rs_camera.launch align_depth:=true enable_pointcloud:=true```

## Setup the conversion of RGBD images to Laser Scans

```roslaunch depthimage_to_laserscan launchfile_sample.launch```

## Setup the navigation node

```roslaunch turtlebot3_navigation turtlebot3_navigation.launch```

## Setting up Parser Based Navigation

```rosrun turtlebot3_navigation talker```

```rosrun turtlebot3_navigation Voice_NLP```