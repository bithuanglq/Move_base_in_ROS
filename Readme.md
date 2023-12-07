### Prerequisite
Ubuntu20.04  
ROS-Noetic  
Gazebo-11  


### Packages
```
sudo apt install ros-noetic-navigation ros-noetic-map-server
```
Change your absolute path of **my_world.pgm** in file (_base_planner/maps/my_world.yaml_)

### Run
Put this repo under your catkin_ws/src
```
cd catkin_ws
mkdir src
cd src
```
Then download this repo and cmake
```
git clone git@github.com:bithuanglq/Move_base_in_ROS.git
cd ..
catkin_make
source devel/setup.bash
roslaunch base_planner navtest.launch
```

### Result
You can specify the end point arbitrarily in rviz, and the robot will independently plan the path and navigate to the end point. The entire process will be displayed in real time in rviz and gazebo.

Click 2D Nav Goal in the upper column and select the target position. The result is as shown below: 
<div align="center">
  <img src="base_planner/result/result.gif" alt="result" width="100%" height="100%" />
</div>
