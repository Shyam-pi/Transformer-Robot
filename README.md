# Transformer-Robot
A novel mobile manipulator with a collapsible arm created for my final project of ENPM662 at the University of Maryland, College Park

Please find the CAD model of the robot in CAD_model.zip 

To run the ROS/URDF package in Gazebo, extract the transformers.zip folder to your catkin workspace, and do the following to build it: 
1. Navigate to your catkin workspace folder, open terminal and enter 'catkin_make' to build the workspace.
2. Enter the following command in your terminal 'source ~/catkin_ws/devel/setup.bash'

Once the building process is done, you can simply launch the package in Gazebo by using the following command in your terminal:
roslaunch transformer template.launch

In order to visualize the feed from the camera, after executing the above command, type 'rviz' in a new terminal window. In your RVIZ, add an 'Image' component, and change the image topic to the available topic, and you can see the video feed from the camera appearing in a window in Rviz.

To launch any of the ROS python scripts, navigate to the scripts folder inside the package, and open a terminal window in that location. Launch any of the available scripts using the below command in terminal 

python3 'script_name.py'

Please take note that you need to use any of the scripts only when Gazebo is running, and terminal window should overlay on top of the Gazebo window.

Following are the description of the available scripts:

1. teleop.py - Use this script to control the mobile base of the robot.
2. publisher.py - It is used to initialize the configuration of the robot. Type 0 followed by the publisher.py to take the robot to collapsed position, and 1 to take it to the extended position.

Please checkout the outputs folder for visualizing the working of the package.

To get comprehensive information on the robot please refer to the report available in the repo.
