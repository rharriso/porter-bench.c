cmake_minimum_required(VERSION 3.3)
project(porter_bench)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES bench_stem.cpp porter/stem.c porter/stem_ISO_8859_1.c porter/stem_UTF_8.c)
add_executable(porter_bench ${SOURCE_FILES})