cmake_minimum_required(VERSION 3.3)
project(porter_bench)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES porter_snowball_bench.cpp porter/stem.c runtime/header.h runtime/api.h runtime/api.c runtime/utilities.c porter_bench.c)
add_executable(porter_snowball_bench ${SOURCE_FILES})
add_executable(porter_bench porter_bench.c)
