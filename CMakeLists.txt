cmake_minimum_required (VERSION 3.8)
project (poisson_blend)

set (CMAKE_CXX_STANDARD 11)

include_directories(src/)

add_executable(poisson_blend src/main.cpp src/lodepng.cpp)

set_target_properties(poisson_blend PROPERTIES VS_DEBUGGER_WORKING_DIRECTORY "${CMAKE_SOURCE_DIR}")