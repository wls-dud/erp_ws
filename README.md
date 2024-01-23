# ERP-42

ERP-42 Gazebo with GPS, IMU, Left/Right Camera, Lidar (Ouster 64ch), Ubuntu 20.04 Ros1 Noetic

```
sudo apt-get install -y ros-noetic-ros-control ros-noetic-ros-controllers ros-noetic-gazebo-ros ros-noetic-gazebo-ros-control ros-noetic-joint-state-publisher-gui ros-noetic-rqt-robot-steering ros-noetic-hector-gazebo-plugins ros-noetic-ackermann-steering-controller -y
sudo apt install -y ros-noetic-cob-perception-msgs ros-noetic-cob-object-detection-msgs # for yolo
sudo apt install ros-noetic-mavros-msgs -y # for gps
sudo apt install sharutils -y # for imu
sudo apt install -y ros-noetic-robot-localization
sudo apt install -y ros-noetic-pcl-ros ros-noetic-rviz ros-noetic-tf2-geometry-msgs # ouster lidar
sudo apt install -y build-essential libeigen3-dev libjsoncpp-dev libcurl4-openssl-dev libspdlog-dev # ouster lidar
sudo apt install -y libv4l-dev
pip install --upgrade python-dateutil # for yolo
sudo apt-get install build-essential git cmake libasio-dev
sudo apt install -y ros-noetic-teleop-twist-keyboard
```
```
cd ~/
git clone https://github.com/wls-dud/erp_ws.git
cd ~/erp_ws
source /opt/ros/noetic/setup.bash
catkin_make
```
---
```
# Gazebo
cd erp_ws
source devel/setup.bash

roslaunch erp42 erp42.launch
```
# erp_ws
