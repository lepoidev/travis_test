cmake_minimum_required(VERSION 3.5.1)
enable_testing()

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

project(travis_test)

set(SOURCES main.cpp)

set(TARGET_NAME test.out)
add_executable(${TARGET_NAME} ${SOURCES})

add_test(NAME test1 COMMAND ${TARGET_NAME})