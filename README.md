# myteleop
This repository contains an ROS package for controlling the turtlebot3 in a simulated environment using teleop controls (WASD). In addition to the standard WASD controls, this package also allows input using the numeric key pad to make precise turns. eg:

"7" is a 45 degree left turn, "4" is a 90 degree left turn

"9" is a 45 degree right turn, "6" is a 90 degree right turn 

"8" is full speed forward, "2" is full speed reverse 

# Package Contents:

  myteleop_key.py (primary file, in nodes folder)
  
  myteleop_key.launch
  
  package.xml
  
  CMakeLists.txt
  
  setup.py
 
  changelog
  
  psuedocode
  
  
  
  
# Requirements:

  ROS (noetic), Gazebo, turtlebot3 packages (https://github.com/ROBOTIS-GIT/turtlebot3)
  
# Running:
  Launch turtlebot3 in simulated gazebo environment eg:
  
  Terminal 1:
  
    $ cd ~/catkin_ws
    
    $ source opt/ros/noetic/setup.bash
    
    $ source ./devel/setup.bash
    
    $ roscore 
    
  Terminal 2:
  
    $ cd ~/catkin_ws
    
    $ source opt/ros/noetic/setup.bash
    
    $ source ./devel/setup.bash
    
    $ TURTLEBOT3_MODEL='waffle
    
    $ roslaunch turtlebot3_gazebo turtlebot3_world.launch 
    
  Terminal 3:
  
    $ cd ~/catkin_ws
    
    $ source opt/ros/noetic/setup.bash
    
    $ source ./devel/setup.bash
    
    $ TURTLEBOT3_MODEL='waffle
    
    $ roslaunch myTeleop myTeleop.launch 
    

