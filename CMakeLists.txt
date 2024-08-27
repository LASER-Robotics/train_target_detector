cmake_minimum_required(VERSION 3.1.2)
project(train_target_detector)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(catkin REQUIRED)

add_definitions(-Wall)
add_definitions(-Wextra)
add_definitions(-Wpedantic)

catkin_package()