cmake_minimum_required(VERSION 2.8.3)
project(cob_lbr)

find_package(catkin REQUIRED COMPONENTS rospy)

## there aren't any messages/services/actions to build

###################################
## catkin specific configuration ##
###################################

catkin_package(
    CATKIN_DEPENDS rospy
    INCLUDE_DIRS #TODO
    LIBRARIES ${PROJECT_NAME}
)

###########
## Build ##
###########

# add include search paths
include_directories(${catkin_INCLUDE_DIRS})

#############
## Install ##
#############

## Mark executables and/or libraries for installation
# install(TARGETS ${PROJECT_NAME}
#   ARCHIVE DESTINATION ${CATKIN_PACKAGE_LIB_DESTINATION}
#   LIBRARY DESTINATION ${CATKIN_PACKAGE_LIB_DESTINATION}
#   RUNTIME DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
# )

# install scripts
install(PROGRAMS scripts/cob_lbr scripts/service_interface.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})