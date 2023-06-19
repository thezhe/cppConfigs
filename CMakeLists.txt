# Copy `./src/**` into the CMake source directory during CMake configure step.

include_guard(GLOBAL)

cmake_minimum_required(VERSION 3.15)
project(CppConfigs)

file(GLOB CXX_CONFIGS "src/**")
file(COPY ${CXX_CONFIGS} DESTINATION ${CMAKE_SOURCE_DIR})
