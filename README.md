# Object Detection in Ros 2 

<p align="center">
 <img src="https://github.com/user-attachments/assets/f34d3f38-1b51-48c7-8455-29192c3b2a8a">
</p>


## Requirements
 - ROS 2 Humble
 - Gazebo 

## Instructions

- Clone the Code somewhere
- Follow Below Instructions for Ros Packages and Paste the Code Respectively
- Add Models in Gazebo's Folder

## Setup and build
```
mkdir -p ~/yolobot/src

cd yolobot/src

ros2 pkg create yolobot_control

ros2 pkg create yolobot_description

ros2 pkg create yolobot_gazebo

ros2 pkg create yolobot_recognition

# Make sure ROS2 is sourced (assuming bash, please replace extension as needed)
source /opt/ros/humble/setup.bash

# Build
colcon build

# Make sure the app is sourced (assuming bash, please replace extension as needed)
source yolobot/install/setup.bash
```

## Run examples
```
ros2 launch yolobot_gazebo yolobot_launch.py

# Open New Terminal
cd /yolobot/src/yolobot_recognition/scripts

python3 ros_recognition_yolo.py
```

## File Structure 

![Screenshot from 2025-02-12 04-07-13](https://github.com/user-attachments/assets/1c35c126-741b-4fd3-b11c-97bef17af12e)

![Screenshot from 2025-02-12 04-08-11](https://github.com/user-attachments/assets/3cfe7bcb-04be-418f-943d-222fb038428d)






