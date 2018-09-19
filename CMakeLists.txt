cmake_minimum_required(VERSION 2.6)
project(evaluate_odometry)

# 添加c++ 11标准支持
set( CMAKE_CXX_FLAGS "-std=c++11")

# source directory
aux_source_directory(./src/ SRC_DIR)

# include directory
include_directories(./include/)

add_executable(evaluate_odometry ${SRC_DIR})

install(TARGETS evaluate_odometry RUNTIME DESTINATION bin)
