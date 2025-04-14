mkdir -p ros2_ws/src
cd ros2_ws
colcon build
cd src
ros2 pkg create my_py_pkg --build-type ament_python --dependencies rclpy
cd ../
colcon build
