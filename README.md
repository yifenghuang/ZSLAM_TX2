# V-SLAM using ZED running under Nvidia TX2. current algorithm is ORB_SLAM2 with RGB-D input


 ## Hardware:
 * Jetson TX2
 * ZED Camera
 
 ## Software:
 * Ubuntu 16.0.4
 * ROS Kinetic
 
 ## Dependencies:
 * Jetson TX2(with a 750 GB SSD. the way to installit  is will update later)
 * ORB SLAM2 - Installed from the instruction [here](https://github.com/raulmur/ORB_SLAM2).
 * ZED Stereo Camera - copy ./zed/src/zed-ros-wrapper to your catkin workspace folder and catkin_make it
 
 ## Running the code
* first untar the ORBvoc.txt in ./SLAM/ORB_SLAM2/Vocabulary
* source setup.bash under your catkin workspace
* roslaunch zed_wrapper zed.launch
* cd ./SLAM/ORB_SLAM2
* rosrun ORB_SLAM2 RGBD Vocabulary/ORBvoc.txt Examples/ROS/ORB_SLAM2/Zed.yaml


## Troubles faced 
