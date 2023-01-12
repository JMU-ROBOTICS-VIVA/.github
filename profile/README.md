# Introduction to Autonomous Robotics

## Introduction
This respository holds projects and other learning material targetted for an undergraduate level
class on introducing autonomous robotics.  It corresponds with a developed course
at James Madision University (CS 354) and the book *Just Enough Robotics* by Nathan Sprague.

Listed below are the general topics covered by the book/course and a brief description 
of the corresponding projects/repositories to support that material.  

Most of these projects incorporate the use of [ROS](ros.org) (Robot Operating System) and have
been tested using the ROS2 Foxy release.

## PID (Proportional, Inverse, Derivative) Controllers
* [**Locomotice_sim**](https://github.com/JMU-ROBOTICS-VIVA/locomotive_sim) 
* **2D PID_Practice Lab** - Activity for learning about multidimensional PID parameters and how to pass in ROS2 
parameters and launch file.  This includes a rocket visualization where the PID controller 
job is to make the rocket climb and maintain a specific altitude.

* **Skibot Programming Assignment** -- Utilizes 2D PID controller and ROS services. 
A skier has a goal location passed via a ROS service and the PID controller must navigate the
skier to this location.  The program must be able to accept new goal locations while running through
ROS interfaces.  A visualization is provided so the student can visualize how well their
controller is functioning.

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
