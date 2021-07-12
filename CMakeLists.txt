cmake_minimum_required(VERSION 3.18)
project(threadpool)
add_compile_options(-std=c++11)
SET(CMAKE_BUILD_TYPE “Debug”)
find_package(Threads REQUIRED)
link_libraries(pthread)
include_directories(include)

add_executable(threadpool src/example.cpp)
