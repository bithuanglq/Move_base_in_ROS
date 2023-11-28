### Prerequisite
Ubuntu20.04  ROS-Noetic gazebo-11


### Packages
'''
sudo apt install ros-noetic-navigation ros-noetic-map-server
'''
Change your absolute path of **my_world.pgm** in file (_base_planner/maps/my_world.yaml_)

### Run
Put this repo in your catkin_ws/src
'''
cd catkin_ws
catkin_make
source devel/setup.bash
roslaunch base_planner navtest.launch
'''

### Result
你可以在rviz中任意指定终点，机器人将自主规划路径并导航至终点，全过程在rviz和gazebo中实时显示

点击上栏的 2D Nav Goal并选定目标位置，结果如下图所示：
<div align="center">
  <img src="base_planner/result/result.gif" alt="result" width="60%" height="100%" />
</div>
