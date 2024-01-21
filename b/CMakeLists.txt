cmake_minimum_required(VERSION 3.10)

project(b)

add_library(b src/b.cpp) 
target_include_directories(b PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include")

add_subdirectory(../a a)
target_link_libraries(b PUBLIC a)
