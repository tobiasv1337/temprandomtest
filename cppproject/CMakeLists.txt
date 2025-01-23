cmake_minimum_required(VERSION 3.25)

# Project name and version
project(cppproject VERSION 1.0)

# Specify C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Add the executable
add_executable(cppproject main.cpp)