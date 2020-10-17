cmake_minimum_required(VERSION 3.0.2)
project(cob_safety_controller)

find_package(catkin REQUIRED)

catkin_package()

install(PROGRAMS bin/safety_controller ros/src/flexisoft_sim.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
