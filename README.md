# Map My World: Udacity RSE Project
#### Onur Bagoren

## Description
The aim of this project is to use RTAB-Map in order to simulate the simultaneous localization and mapping (SLAM) with in an unknown environment that was built and simulated in a Gazebo environment.

## Setup

### Installation
If the catkin_ws does not exists:
1. `cd ~`
2. `mkdir -p catkin_ws/src; cd catkin_ws/src`
3. `catkin_init_workspace`
4. `cd ../; catkin_make`
5. `cd src`
6. `git clone git@github.com:onurbagoren/slam.git`

### Execution
Open 3 tabs from the terminal. Initially run `cd ~/catkin_ws; source devel/setup.bash` on each tab.
On the first tab:
`roslaunch slam mapping.launch`
On the second tab:
`roalaunch slam worl.launch`

These two tabs will start up 3 windows: RVix, Gazebo and RTAB-Map

In order to drive the robot, on the third tab:
`roslaunch slam teleop.launch`
