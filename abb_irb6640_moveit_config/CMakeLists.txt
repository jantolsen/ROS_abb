cmake_minimum_required(VERSION 3.0.2)
project(abb_irb6640_moveit_config)
add_definitions(-std=c++11)

find_package(catkin REQUIRED)

catkin_package()

install(DIRECTORY launch DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
install(DIRECTORY config DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
