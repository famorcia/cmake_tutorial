cmake_minimum_required(VERSION 3.23)

project(02_minimal_with_a_lib)

set(CMAKE_CXX_STANDARD 11)


add_library(
        my_lib  # library name
        my_lib.cpp  # list of file to be used in the library
)

add_executable( 02_minimal_with_a_lib  main.cpp )

target_link_libraries(
        02_minimal_with_a_lib # name of the target (the same as executable in this case)
        my_lib  # name of the lib
)

