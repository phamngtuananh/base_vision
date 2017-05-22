Adding package into workspace:


	cd ~/catkin_ws/src/

	git clone https://github.com/phamngtuananh/base_vision.git

	cd ~/catkin_ws/src/base_vision/cfg

	chmod a+x armor_color.cfg board_color.cfg building_blocks.cfg

	cd ~/catkin_ws

	catkin_make


Running the red ball targetting node:


	roslaunch base_vision target.launch

The output will be shown on screen, and also via topic /center, which is of type Vector3


To run the camera: make sure you have the usb_cam package in the workspace


To add the package into workspace:

	cd ~/catkin-ws/src

	git clone https://github.com/bosch-ros-pkg/usb_cam.git

	cd ..

	catkin_make


To run the camera

	roslaunch base_vision usb_cam.launch