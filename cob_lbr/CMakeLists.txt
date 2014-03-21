# http://ros.org/doc/groovy/api/catkin/html/user_guide/supposed.html
cmake_minimum_required(VERSION 2.8.3)
project(cob_lbr)
# Load catkin and all dependencies required for this package
# TODO: remove all from COMPONENTS that are not catkin packages.
find_package(catkin REQUIRED COMPONENTS actionlib cob_srvs brics_actuator trajectory_msgs sensor_msgs diagnostic_msgs)


catkin_package(
    DEPENDS actionlib cob_srvs brics_actuator trajectory_msgs sensor_msgs diagnostic_msgs 
    CATKIN_DEPENDS # TODO
    INCLUDE_DIRS # TODO include
    LIBRARIES # TODO
)

install(DIRECTORY common/
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/common
)

install(DIRECTORY src/
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/src
)

install(PROGRAMS src/service_interface.py bin/cob_lbr
  DESTINATION ${CATKIN_PACKAGE_LIB_DESTINATION}
)

