# set the minimum versione required (at least 3.0 is suggested)
cmake_minimum_required(VERSION 3.23)

# set the name of the project
project(01_minimal)

# set the standard to be required (is optional)
set(CMAKE_CXX_STANDARD 11)

# how to debug: message
message("Hello world")

# build an executable with a name
add_executable(
        01_minimal  # name of executable
        main.cpp    # list of file to be compiled
)
