# Deep-Visual-Odometry
To use this CNN model, the following steps are required:

1) Download the environment from https://github.com/Gastd/p3at_tutorial.

2) Add the monocular camera to this model by following the steps for adding sensors as outlined on the official ROS page. Additionally, place the robot at the following coordinates with the following orientation:  
   x = -9, y = -9, Yaw = 0.0.

3) Run the following in separate terminals:

   a) Master node.
   
   b) Environment: pioneer3at.gazebo.launch.
   
   c) Move Base: move_base_mapless_demo.launch.

   d) Run the gmapping node.

   e) Open the CNN model and input the colour monocular image from the camera published on the topic /pioneer3at/camera/image_raw.

   f) Publish the poses.csv file to the /waypoint_markers topic and start the move_base server so it can choose a path for the robot to follow.
