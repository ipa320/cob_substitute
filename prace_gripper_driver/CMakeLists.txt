cmake_minimum_required(VERSION 2.8.3)
project(prace_gripper_driver)

find_package(catkin REQUIRED)

catkin_package()

install(DIRECTORY ros
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
