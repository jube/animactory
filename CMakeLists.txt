cmake_minimum_required(VERSION 2.8)

project(ANIMACTORY)

include(GNUInstallDirs)

find_package(Qt5Core REQUIRED)
find_package(Qt5Gui REQUIRED)

add_definitions(-Wall -g -O2)
add_definitions(-std=c++11)

add_subdirectory(code)
