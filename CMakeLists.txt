# Copy `./src/*` into the CMake source directory.

cmake_minimum_required(VERSION 3.15)
project(cppConfigs VERSION 1.0.0)

file(GLOB CXX_CONFIGS "src/*")
file(COPY ${CXX_CONFIGS} DESTINATION ${CMAKE_SOURCE_DIR})
