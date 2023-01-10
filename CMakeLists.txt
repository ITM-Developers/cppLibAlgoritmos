cmake_minimum_required(VERSION 3.14)

project(algoritmos LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(algoritmos SHARED
  algoritmos_global.h
  algoritmos.cpp
  algoritmos.h
)

target_compile_definitions(algoritmos PRIVATE LIBALGORITMOS_LIBRARY)
