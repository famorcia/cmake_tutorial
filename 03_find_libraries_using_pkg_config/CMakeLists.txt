cmake_minimum_required(VERSION 3.23)

project(03_find_libraries_using_pkg_config)

set(CMAKE_CXX_STANDARD 11)

# add package for config
find_package(PkgConfig REQUIRED)

# packages can be added with env variable PKG_CONFIG_PATH
# for example export PKG_CONFIG_PATH=${PKG_CONFIG_PATH}:/your_path/pkgconfig
pkg_check_modules (
        LIBELF   # variable will be used by cmake
        REQUIRED        # is required mandatory
        IMPORTED_TARGET # use as target
        libelf  # name of package to be found
)

add_executable( 03_find_libraries_using_pkg_config  main.cpp )

target_link_libraries(
        03_find_libraries_using_pkg_config
        ${LIBELF_LIBRARIES}
)

