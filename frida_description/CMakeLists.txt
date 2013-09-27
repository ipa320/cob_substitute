cmake_minimum_required(VERSION 2.8.3)
project(frida_description)

find_package(catkin REQUIRED)

## there aren't any messages/services/actions to build

###################################
## catkin specific configuration ##
###################################

catkin_package()

#############
## Install ##
#############

# Install urdf files
install(DIRECTORY urdf/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/urdf)