# beginner_tutorials
UMD ENPM808X ROS Beginner Tutorials

## Overview
This project contains a complete ROS catkin build system workspace with a single
ROS package called "beginner_tutorials."  The catkin workspace is set up as an Eclipse IDE project
for editing/building convenience.  The package and code is taken directly from the Core ROS Tutorials
found at http://wiki.ros.org/ROS/Tutorials.

## Pre-requisites
This ROS catkin workspace and ROS package have been built and tested for the Indigo-Igloo release of
the Robot Operating System.  In order to build and execute this package, you will need to have
ROS Indigo-Igloo installed on your system, along with the ROS dependencies identified in the
package.xml manifest file (roscpp, rospy, and std_msgs).  The instructions in this README.md file
assume that you are already familiar with ROS, the ROS catkin build system, and the Eclipse IDE.

## Import into Eclipse IDE to edit and/or build
To import the project into the Eclipse IDE: clone or download this repository to your
local machine, then use the Eclipse File -> Import -> General -> Existing Projects
into Workspace function; press Next, then browse to the catkin_ws/build directory, and
press Finish (do not select "Copy projects into workspace").  If imported properly,
the Eclipse Project -> Build Project function will run the catkin_make command to build
the workspace.

Note that this will import the entire catkin workspace contained in this repository as a project into
your Eclipse IDE, not just the beginner_tutorials ROS package.

## Building outside the Eclipse IDE
If you would like to build the ROS package outside of the Eclipse IDE: clone or download this
repository to your local machine, then set your working directory to the catkin_ws subdirectory and
issue the command "catkin_make" to build the workspace.

## Running the tutorial programs
The ROS package beginner_tutorials contains two programs, a ROS publisher called "listener" and a
ROS subscriber called "publisher."  To run them, first make sure that this workspace has been
added to your local ROS configuration by executing the catkin_ws/build/setup.bash script in each
terminal window from which you will invoke one of the programs.  Then, use the command
"rosrun beginner_tutorials listener" to run the subscriber program, and "rosrun beginner_tutorials talker"
to run the publisher program.
