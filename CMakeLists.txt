# Copyright (c) 2024
# Commonwealth Scientific and Industrial Research Organisation (CSIRO)
# ABN 41 687 119 230
#
# Author: David Haddon <had067@csiro.au>

cmake_minimum_required(VERSION 3.10)

project(JoyStick)

# Catkin
find_package(catkin REQUIRED)
catkin_package()


# Install
add_library(${PROJECT_NAME} INTERFACE)
install(TARGETS
    ${PROJECT_NAME}
  PUBLIC_HEADER DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
