cmake_minimum_required(VERSION 3.0.2)
project(hgailab_ros)

find_package(catkin REQUIRED COMPONENTS
  cv_bridge
  geometry_msgs
  message_runtime
  rospy
  sensor_msgs
  std_msgs
)

add_message_files(
  FILES
    BoundingBox.msg
    BoundingBoxes.msg
)

generate_messages(
  DEPENDENCIES
    geometry_msgs
    sensor_msgs
    std_msgs
)

catkin_package()

include_directories()