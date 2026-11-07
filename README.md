<!-- ABOUT THE PROJECT -->
## About The Project

This project is for our Applied Machine Learning (CST8504) Assignment2 ROS2
hand gesture control of create3 robot.

<!-- REQUIREMENTS -->
## Requirements
In Linux, python (ROS2, opencv, mediapipe)


1) mkdir your_ws      #create your new workspace
2) cd your_ws
3) mkdir src
4) cd src
5) clone git repo here

# Now to install the python packages
6) cd ~/your_ws
7) sudo apt update
   pip3 install "numpy>=2"  
   pip3 install opencv-python-headless  opencv-contrib-python
   pip3 install mediapipe
   sudo apt-get install libgles2   

8) colcon build       # it will create new dirs and compile code.
9) source install/setup.py

# Run the first node test
10) ros2 run aisd_vision py_node




<!-- DEPLOYMENT -->
## DEPLOYMENT

To deploy and run the project in a demonstration environment:

1. Ensure all requirements are installed and the workspace is built as described above.
2. Source your ROS2 workspace:
   ```
   source ~/your_ws/install/setup.bash
   ```
3. Connect your Create3 robot and ensure it is powered on and accessible.
4. Launch the gesture control node:
   ```
   ros2 run aisd_vision gesture_publisher
   ```
5. In another terminal:
   - Run step 2 above.
   - Launch the gesture control node:
   ```
   ros2 run aisd_vision motion_listener
   ```   



<!-- TEAM -->
## TEAM
    K. Tam
    G. Byron

<!-- ACKNOWLEDGEMENTS -->
## ACKNOWLEDGEMENTS
