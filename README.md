# Al-week2

This time we will clone an existing project on github and run the robotic arm by it

First we start by copying these instructions into the workspace

$ rosdep install--from-paths src--ignore-src-r-y

Then prove this packages :

$ sudo apt-get install ros-melodic-moveit

$ sudo apt-get install ros-melodic-joint-state-publisher rosmelodic-joint-state-publisher-gui

$ sudo apt-get install ros-melodic-gazebo-ros-control jointstate-publisher

$ sudo apt-get install ros-melodic-ros-controllers ros-melodicros-control

after that configuring Arduino by install Arduino IDE in ubuntu through https://www.arduino.cc/en/software to install
run $ sudo ./install.sh after unzipping the folder

next launch Arduino IDE by Install the arduino package and ros library
http://wiki.ros.org/rosserial_arduino/Tutorials/Arduino%20IDE%20Setup

note: make sure to change the port permission before uploading the Arduino code

$ sudo chmod 777/dev/ttyUSB0

Finally the arm will be controlled:

by joint_state_publisher 

$ roslaunch robot_arm_pkg check_motors.launch

![photo_2022-08-01_20-59-51](https://user-images.githubusercontent.com/108091010/182212480-a9acc894-c0f5-473a-8106-cb750a53df0f.jpg)

by moveit and kinematics 

$ roslaunch moveit_pkg demo.launch

![photo_2022-08-01_20-59-54](https://user-images.githubusercontent.com/108091010/182212514-896f739c-1371-4241-bcb9-0bdfdc5444ea.jpg)


