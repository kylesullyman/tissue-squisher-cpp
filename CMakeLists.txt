cmake_minimum_required(VERSION 4.2)
project(tissue_squisher_cpp)

# set(CMAKE_CXX_STANDARD 14)

include_directories(.)

find_package(fmt CONFIG REQUIRED)

add_executable(tissue_squisher_cpp
        main.cpp
        main.h
        README.md
        vcpkg-configuration.json
        vcpkg.json)

target_link_libraries(tissue_squisher_cpp PRIVATE fmt::fmt)

