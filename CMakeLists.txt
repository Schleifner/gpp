cmake_minimum_required(VERSION 3.1)

project(gpp)

set(CMAKE_CXX_FLAGS "-std=c99 ${CMAKE_CXX_FLAGS}")

include_directories(${CMAKE_CURRENT_SOURCE_DIR})
add_definitions(-DHAVE_CONFIG_H)

set(sourceFiles src/gpp.c)

add_executable(gpp ${sourceFiles})