cmake_minimum_required(VERSION 3.10)

project(a)

add_library(a src/a.cpp)
target_include_directories(a PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include")
