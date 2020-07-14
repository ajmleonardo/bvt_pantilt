cmake_minimum_required(VERSION 2.8.3)
project(bvt_pantilt)

find_package(catkin REQUIRED COMPONENTS
  rospy
  std_msgs
  message_generation
)

add_message_files(
  FILES
  PanTiltOrientation.msg
 )

generate_messages( #Required for the service's message
   DEPENDENCIES
   std_msgs
 )

catkin_package()



