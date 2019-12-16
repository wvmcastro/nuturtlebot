cmake_minimum_required(VERSION 2.8.3)
project(nurtle)

find_package(catkin REQUIRED COMPONENTS message_generation roscpp)

add_message_files(
   FILES
   WheelVelocities.msg
)

generate_messages(
   DEPENDENCIES
)

catkin_package(CATKIN_DEPENDS message_runtime)

