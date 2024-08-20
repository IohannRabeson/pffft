cmake_minimum_required(VERSION 3.9)

project(Pffft LANGUAGES C)

add_library(Pffft STATIC pffft.h pffft.c)
target_include_directories(Pffft PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
add_definitions(-D_USE_MATH_DEFINES)