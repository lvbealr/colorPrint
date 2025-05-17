cmake_minimum_required(VERSION 3.10) 

project(colorPrint LANGUAGES CXX)

add_library(colorPrint STATIC colorPrint.cpp)

target_include_directories(colorPrint PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

set_target_properties(colorPrint PROPERTIES POSITION_INDEPENDENT_CODE ON)