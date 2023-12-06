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

Some things after that fail, like in this tutorial: https://roboticscasual.com/de/ros-tutorial-ur5-roboter-steuern-mit-ros_control-pid-regler-tuning-erklart/#kurzanleitung-ros_control, which fails when trying to use the last command for gazebo. 
