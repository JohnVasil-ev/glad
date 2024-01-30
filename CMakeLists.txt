cmake_minimum_required(VERSION 3.15)

project(libglad
    DESCRIPTION "Generated glad lib"
    LANGUAGES C)

set(PROJECT_SOURCE_DIR "${CMAKE_CURRENT_SOURCE_DIR}/src")

add_library(glad "${PROJECT_SOURCE_DIR}/gl.c")

target_include_directories(glad PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include")
