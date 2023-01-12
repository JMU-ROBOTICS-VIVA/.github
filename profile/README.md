# Introduction to Autonomous Robotics

## Introduction
This respository contains projects, template program and utilities, and other learning material
targetted for an undergraduate level
class on introducing autonomous robotics.  It corresponds with a developed course
at James Madision University (CS 354) and the book *Just Enough Robotics* by Nathan Sprague.

Listed below are the general topics covered by the book/course and a brief description 
of the corresponding projects/repositories to support that material.  

Some of these projects incorporate the use of [ROS](ros.org) (Robot Operating System) and have
been tested using the ROS2 Foxy release.  Where applicable, these projects utilize the
[Turtlebot-3 Waffle Pi](https://www.robotis.us/turtlebot-3/) robot platform.

## PID (Proportional, Inverse, Derivative) Controllers

* [**Locomotice_sim** Lab](https://github.com/JMU-ROBOTICS-VIVA/locomotive_sim). A one
dimensional train needs to stop at a point on the track and the only control 
the student can apply is a force (both positive and negative).  The student
attempts to accomplish this by hand to motivate the need for a controller.

* [**2D PID_Practice** Lab](https://github.com/JMU-ROBOTICS-VIVA/rocketbot) - Activity for learning about multidimensional PID parameters and how to pass in ROS2 
parameters and launch file.  This includes a rocket visualization where the PID controller 
job is to make the rocket climb and maintain a specific altitude.

* [**Skibot Programming Assignment**](https://github.com/JMU-ROBOTICS-VIVA/Skibot_navigation)(https://github.com/JMU-ROBOTICS-VIVA/Skibot_navigation))  -- Utilizes 2D PID controller and ROS services. 
A skier has a goal location passed via a ROS service and the PID controller must navigate the
skier to this location.  The program must be able to accept new goal locations while running through
ROS interfaces.  This interface also introduces a angular/rotational force term.
A visualization is provided so the student can visualize how well their
controller is functioning. Files for the GUI and other support files the student will not need
to change are located in the main [Skibot](https://github.com/JMU-ROBOTICS-VIVA/skibot) reposotory.

## Planning

* [**PyArm**](https://github.com/JMU-ROBOTICS-VIVA/py_arm) A 2D robotic arm simulator that
can be used to develop and test planning algorithms.

* [**A\*, RRT and RRT* Planning**](https://github.com/JMU-ROBOTICS-VIVA/rrt_rrtstar) Allows
students to explore using a deterministic and optimal planner (A*) versus a few probablistic
ones.  Uses the [**PyArm**](https://github.com/JMU-ROBOTICS-VIVA/py_arm) for visualization.

## Navigation

* [**Random Navigation Lab** ](https://github.com/JMU-ROBOTICS-VIVA/random_nav).  Utilizes ROS
navigation and occupancy grids.  Students select a location via the ROS *RViz* utility,
which then communicates with the student agent which is responsible for working
with the ROS navigation system to move the robot to the goal configuration.

* [**Zeta -- A Navigation Challenge Project**](https://github.com/JMU-ROBOTICS-VIVA/zeta_all)
This project involves conducted a time limited search to "rescue" indidivuals, each marked
with an aruco tag and identified from the robot's camera.  A ROS occupancy map is provided
at the competition (but not before, so, essentially it is an unknown space).  It has
been tested with the [Turtlebot-3 Waffle Pi](https://www.robotis.us/turtlebot-3/).
Many aspects of this project can be enhanced, for example, computer vision methods can
be employed to better spot individuals from far away.  The supporting respositories 
that contain Zeta in the name are in support of this project.

## ROS and Turtlebot Supoprt Packages

These packages augment the ROS2 *Foxy* programming Python API language and
the [Turtlebot-3 Waffle Pi](https://www.robotis.us/turtlebot-3/) platform to support
the projects/labs.

* [**Transform service**](https://github.com/JMU-ROBOTICS-VIVA/transform_service) 
A tf interface for Python that provides transforms between frames.

* [**JMU ROS utilities**](https://github.com/JMU-ROBOTICS-VIVA/jmu_ros2_util) Supplies
transform and a few functions for making it easier to work with OccypancyGrid msgs.

* [**JMU Turtlebot3 Bringup**](https://github.com/JMU-ROBOTICS-VIVA/jmu_turtlebot3_bringup) 
This package makes the Turtlebot code more ROS2 *Foxy* friendly.

* [**Ros2_Aruco**](https://github.com/JMU-ROBOTICS-VIVA/ros2_aruco) Wrapper
for OpenCV Aruco Marker tracking for use with ROS2.
