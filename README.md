# Lab 4
## Modern Robotics Programming
---
### Launch File
To use the launch file, download the package, rebuild your catkin\_environment, and source devel/setup.bash.  Then, the launch file can be run by:  `roslaunch lab4_urdf_package display.launch`.  The parameters for the launch file are listed below.

1. `use_xacro`:  *Optional*, Default is *false*  If true, must pass in a filename to a .xacro file.  Otherwise, pass in a filename to a .urdf file.
1. `use_gui`:  *Optional*, Default is *true*  If true, launches joint\_state\_publisher and sets the \\use_gui param to *true*.
1. `filename`:  *Optional*, Default is *robot.xacro* or *robot.urdf* depending on the `use_xacro` argument.

The default launch file starts RVIZ with the joint\_state\_publisher.  To launch without RVIZ and the joint\_state\_publisher, run `roslaunch lab4_urdf_package display.launch use_gui:=false`

### Dependencies
* catkin
* roscore
* gazebo_plugins
* joint_state_publisher
* xacro
* rviz

### Other Comments
I changed the visual geometry of the robot to better reflect the visual of the platform itself.  However, the collision box remains the same as the entirety of the box.
