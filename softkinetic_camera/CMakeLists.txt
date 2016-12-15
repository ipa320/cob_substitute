cmake_minimum_required(VERSION 2.8.3)
project(softkinetic_camera)

find_package(catkin REQUIRED)

catkin_package()

install(PROGRAMS bin/softkinetic_bringup_node
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
