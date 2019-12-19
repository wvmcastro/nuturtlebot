cmake_minimum_required(VERSION 2.8.3)
project(nuturtlebot)

find_package(catkin REQUIRED COMPONENTS message_generation roscpp std_msgs)

add_message_files(
   FILES
   SensorData.msg
   WheelCommands.msg
)

generate_messages(
  DEPENDENCIES
  std_msgs
)

catkin_package(CATKIN_DEPENDS message_runtime std_msgs)

