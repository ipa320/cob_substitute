cmake_minimum_required(VERSION 2.8.3)
project(cob_lbr)

find_package(catkin REQUIRED COMPONENTS)

catkin_package()

install(DIRECTORY common
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

install(PROGRAMS src/service_interface.py
    DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}/src
)

install(FILES bin/cob_lbr
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}/bin
)

