cmake_minimum_required(VERSION 3.0.2)
project(abb_irb2400_support)

find_package(catkin REQUIRED)

catkin_package()

if (CATKIN_ENABLE_TESTING)
  find_package(roslaunch REQUIRED)
  roslaunch_add_file_check(tests/roslaunch_test_2400.xml)
  roslaunch_add_file_check(tests/roslaunch_test_2400_12_155.xml)
endif()

install(DIRECTORY config launch meshes urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
