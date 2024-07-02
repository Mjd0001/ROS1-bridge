# ROS1-bridge
## Workspace Creation in ROS1 Noetic And ROS2 Humble
### ROS1
```
$ source /opt/ros/noetic/setup.bash
$ mkdir -p ~/catkin_ws/src
$ cd ~/catkin_ws/
$ catkin_make
$ source devel/setup.bash
```
### ROS2
```
source /opt/ros/foxy/setup.bash
mkdir -p ~/ros2_ws/src
cd ~/ros2_ws
colcon build
```

## Install Arduino robot Arm packagre in ros noetic
Clone this projcet https://github.com/smart-methods/arduino_robot_arm.git using the followwing commands:
```
cd catkin_ws/src/
git clone https://github.com/smart-methods/arduino_robot_arm.git
```
then go back and catkin the workapace:
```
cd ..
catkin_make
```
try this command to make sure everything is correct:
```
roslaunch robot_arm_pkg check_motors.launch
```
