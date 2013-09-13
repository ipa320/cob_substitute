cmake_minimum_required(VERSION 2.8.3)
project(cob_lbr)

find_package(catkin REQUIRED COMPONENTS rospy)

## there aren't any messages/services/actions to build

###################################
## catkin specific configuration ##
###################################

catkin_package()

#############
## Install ##
#############

# install scripts
install(PROGRAMS scripts/cob_lbr scripts/service_interface.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
  USE_SOURCE_PERMISSIONS)