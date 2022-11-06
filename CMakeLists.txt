cmake_minimum_required(VERSION 3.0.0)
project(opencv VERSION 0.1.0)

find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})
add_executable(opencv main.cpp)
target_link_libraries(opencv ${OpenCV_LIBS})

set_property(TARGET opencv PROPERTY CXX_STANDARD 17)