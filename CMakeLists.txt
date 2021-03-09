cmake_minimum_required(VERSION 3.0 FATAL_ERROR)

project(tinythreadcpp)

add_library(tinythreadcpp STATIC
	"${CMAKE_SOURCE_DIR}/source/fast_mutex.h"
	"${CMAKE_SOURCE_DIR}/source/tinythread.cpp"
	"${CMAKE_SOURCE_DIR}/source/tinythread.h"
)

target_include_directories(tinythreadcpp PUBLIC "${CMAKE_SOURCE_DIR}/source")