# My World

`myworld` is a project that utilizes [gazebo](http://gazebosim.org/) (7.x) with [ROS](https://www.ros.org/) (Kinetic) to create a 3D world.

![Final result](./images/final.png)


## How to run

This project has been tested using Ubuntu 16.04 LTS

### Set-up: Install ROS 1 Kinetic and Gazebo. (If you have ROS and Gazebo already installed, skip set-up)
1. Clone this repository through terminal: `git clone https://github.com/martinezedwin/myworld.git`
2. [Install ROS 1](https://www.ros.org/). In this case since we are using [Ubuntu 16.04 LTS](http://releases.ubuntu.com/16.04/), we will use ROS Kinetic. You can also install this using the `ros_install.sh` script in this repository (i.e. run this command in terminal: `sudo chmod +x ros_install.sh && ./ros_install.sh`) Refer to the website for installation if this does not work.
3. [Install Gazebo](http://gazebosim.org/tutorials?tut=ros_installing&cat=connect_ros): `sudo apt-get install ros-kinetic-gazebo-ros-pkgs ros-kinetic-gazebo-ros-control`. Refer to the website for installation if this does not work.
4. Run `gazebo` to ensure it's working properly.


### How to run (After cloning repository)
1. `cd PATH/TO/myworld`
2. `cmake . && make`
3. `export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/PATH/TO/myworld/`
4. `cd world`
5. `gazebo myworld.world`
