cmake_minimum_required(VERSION 3.3)
project(porter_bench)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -c -std=c++11")

include_directories(runtime porter)
set(SOURCE_FILES porter_bench.cpp porter/stem.c)
set(HEADER_FILES runtime/header.h runtime/api.h)

add_executable(porter_bench ${SOURCE_FILES} ${HEADER_FILES})