# elissa3_ur10e_controller
**ROS controller design for UR10e robot manipulator arms**

The most basic ROS related topics can be learned in https://www.youtube.com/watch?v=d_3eUj3yDwg&list=PLWmIJlISEj2OqSieZYqZ4nmoBmubT8OGR, which is a german tutorial for ROS.
For installing the Universal Robots (UR) package the site https://github.com/ros-industrial/universal_robot can be used.

To view a UR ROS manipulator arm in RViz use the following commands.

```ruby
roscore
```
```ruby
roslaunch ur_description view_ur10e.launch
```
And then open a config window to influence the joints:
```ruby
roslaunch ur10e_moveit_config moveit_planning_execution.launch
```

This tutorial describes a simple position controller for the UR5 manipulator arm https://roboticscasual.com/de/ros-tutorial-ur5-roboter-steuern-mit-ros_control-pid-regler-tuning-erklart/#kurzanleitung-ros_control. Doing it for the UR10e by using the following commands.

Create new package:
```ruby
catkin_create_pkg ur10e_simple_controller
```
Then I changed up the files according to the UR10e.

The UR5 example fails at the last line for me and I still get alot of errors with my own try for the UR10e.
