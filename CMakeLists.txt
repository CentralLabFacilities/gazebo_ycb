cmake_minimum_required(VERSION 2.8.3)
project(gazebo_ycb)

find_package(catkin REQUIRED)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES gazebo_ycb
#  CATKIN_DEPENDS other_catkin_pkg
#  DEPENDS system_lib
)

#############
## Install ##
#############

install(DIRECTORY models
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

catkin_add_env_hooks(${PROJECT_NAME} 
  SHELLS sh 
  DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/env-hooks)
