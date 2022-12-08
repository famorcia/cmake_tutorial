# run cmake with -DCMAKE_VERBOSE_MAKEFILE=ON

cmake_minimum_required(VERSION 3.23)

project(04_debug_cmake)

set(CMAKE_CXX_STANDARD 11)

# how to debug: message
message("04_debug_cmake")

# how to debug: fatal that stop cmake processing
#message(FATAL_ERROR "This is a fatal error message")

add_executable(04_debug_cmake  main.cpp)
