# set the minimum versione required (at least 3.0 is suggested)
cmake_minimum_required(VERSION 3.23)

# set the name of the project
project(cmake_examples)

add_subdirectory(01_minimal)
add_subdirectory(02_minimal_with_a_lib)
add_subdirectory(03_find_libraries_using_pkg_config)
add_subdirectory(04_debug_cmake)
