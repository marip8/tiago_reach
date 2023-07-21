cmake_minimum_required(VERSION 3.0.2)
project(tiago_reach)

find_package(catkin REQUIRED)

catkin_package()

foreach(dir config model results)
  install(DIRECTORY ${dir}/ DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/${dir})
endforeach()
