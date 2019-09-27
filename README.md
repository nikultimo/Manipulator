# HomeWork1FRP
Modelling the robot(Manipulator)

-
DESCRIPTION: 
-
In this project i model the Toshiba Manipilator with end-effector, wishing to control its moving to gather smth or do other work via its grabber. It's very useful project for me because I'm interested in manipulators and how to control them, make to move. Characteristics of the manipulator could be changed in urdf/ xacro file by varying parameters.

-
GOALS:
-
-Introduce to ROS, Gazebom, Rviz, urdf, xacro editing
-Improving skills of modelling robots
-Introducing to manipulators

-
HOW TO RUN THE PROJECT?
-
1) Open the terminal
2) type "mkdir catkin"
3) type "cd catkin"
4) type "mkdir src"
5) type "catkin_make"
6) type "cd src"
7) type "catkin_create_pkg box_robots"
8) type "cd box_robots"
9) type "mkdir src launch urdf"
10) type "cd .." 2 times
11) put file "box_robots.xacro" in /catkin/src/box_robots/urdf
12) put file "box_robots.urdf" in /catkin/src/box_robots/urdf
13) put file display.launch" in /catkin/src/box_robots/launch
14) type "catkin_make" in "catkin" directory
# Rviz
15) type "export LC_NUMERIC="en_US.UTF-8"" (to allow decimal numirals)
16) type "source devel/setup.bash"
17) type "roslaunch box_robots display.launch" (may be, it's needed to do twice if RVIZ doesn't work correctly)
(Push Ctrl-z)
# Gazebo
18) type "roslaunch gazebo_ros empty_world.launch"
19) Open new tab
20) type "catkin_make"
21) type "source devel/setup.bash"
22) type "rosrun gazebo_ros spawn_model -urdf -file `rospack find box_robots`/urdf/box_robots.urdf -model Manipulator"
(22: don't forget '' (edit this file and copy 22 line)
