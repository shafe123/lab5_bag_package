# Lab 5
## Modern Robotics Programming
#### Contributors: Ethan Shafer (ehs70), Naomi Hourihane (jdh156), Tejaswini Rajkumar(txr177)
---
### Launch File
To use the launch file, download the package, rebuild your catkin\_environment, and source devel/setup.bash.  Then, the launch file can be run by:  `roslaunch lab5_bag_package display.launch`.  The parameters for the launch file are listed below.

1. `use_xacro`:  *Optional*, Default is *false*  If true, must pass in a filename to a .xacro file.  Otherwise, pass in a filename to a .urdf file.
1. `use_old_robot_xacro`:  *Optional*, Default is *false*  If true, the filename for `use_xacro` will be set to `old_robot.xacro`.  This option must be set with `use_xacro = true` to be utilized.
1. `use_gui`:  *Optional*, Default is *true*  If true, launches joint\_state\_publisher and sets the \\use_gui param to *true*.
1. `use_robot_state_publisher`:  *Optional*, Default is *true*.  Turns on or off the robot state publisher.
1. `use_sim_time`: *Optional*, Default is *true*.  Utilizes the bag clock time for visualization.
1. `file`:  *Optional*, Default is *robot.xacro* or *robot.urdf* depending on the `use_xacro` argument.
1. `rviz_file`:  *Optional*, Default is `$(find lab5_bag_package)/config/config.rviz` Specifies the rviz configuration file for viewing the simulation.

### Dependencies
* catkin
* roscore
* gazebo_plugins
* joint\_state\_publisher
* xacro
* rviz
