cmake_minimum_required(VERSION 3.25)

# Project name and version
project(MyProject VERSION 1.0)

# Specify C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Enable warnings for GCC and Clang
if (CMAKE_CXX_COMPILER_ID MATCHES "GNU|Clang")
    add_compile_options(-Wall -Wextra -pedantic)
elseif (CMAKE_CXX_COMPILER_ID MATCHES "MSVC")
    # Enable warnings and treat them as errors for MSVC
    add_compile_options(/W4 /WX)
endif()

# Add the executable
add_executable(MyProject main.cpp)