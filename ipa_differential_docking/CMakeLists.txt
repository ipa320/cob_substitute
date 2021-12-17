cmake_minimum_required(VERSION 3.0.2)
project(ipa_differential_docking)

find_package(catkin REQUIRED)

catkin_package()

install(PROGRAMS bin/${PROJECT_NAME}_node
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
