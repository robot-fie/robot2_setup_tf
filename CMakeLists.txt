cmake_minimum_required(VERSION 3.0.2)
project(robot2_setup_tf)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  tf2
  tf2_ros
)

catkin_package(
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

install(DIRECTORY launch/ 
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
