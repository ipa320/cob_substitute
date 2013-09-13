cmake_minimum_required(VERSION 2.8.3)
project(frida_description)

find_package(catkin REQUIRED)

## there aren't any messages/services/actions to build

###################################
## catkin specific configuration ##
###################################

catkin_package(
    CATKIN_DEPENDS #TODO
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

# Install urdf files
install(DIRECTORY urdf/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/urdf)