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