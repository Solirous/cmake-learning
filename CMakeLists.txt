cmake_minimum_required(VERSION 3.10)

project(test VERSION 1.0)

add_executable(${PROJECT_NAME} ./main.cpp ./engine.cpp)

target_include_directories(${PROJECT_NAME} PUBLIC &<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>/include)