cmake_minimum_required(VERSION 3.5)
project(libcbdetect)

find_package(catkin REQUIRED)
find_package(OpenCV REQUIRED)

catkin_package(INCLUDE_DIRS
               include
               LIBRARIES
               cbdetect)

include_directories(include ${OpenCV_INCLUDE_DIRS})

add_subdirectory(${PROJECT_SOURCE_DIR}/src)
add_subdirectory(${PROJECT_SOURCE_DIR}/src/libcbdetect)