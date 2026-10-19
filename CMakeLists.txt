cmake_minimum_required(VERSION 3.21)
project(UndergroundTestConsole VERSION 1.0.0)

# Geode's SDK toolchain is normally configured by the Geode CLI / IDE setup.
include($ENV{GEODE_SDK}/cmake/Geode.cmake)

add_library(${PROJECT_NAME} SHARED src/main.cpp)
setup_geode_mod(${PROJECT_NAME})
