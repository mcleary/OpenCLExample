cmake_minimum_required(VERSION 3.10)

project(OpenCLExample)

find_package(OpenCL REQUIRED)

add_executable(OpenCLExample "OpenCLExample.cpp")
target_include_directories(OpenCLExample PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})

target_link_libraries(OpenCLExample OpenCL::OpenCL)
