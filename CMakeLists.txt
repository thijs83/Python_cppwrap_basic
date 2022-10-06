cmake_minimum_required(VERSION 3.4...3.18)
project(cmake_example)

find_package(Eigen3 REQUIRED)
include_directories(${EIGEN3_INCLUDE_DIRS})

add_subdirectory(pybind11)
pybind11_add_module(ComplexCpp src/ComplexCpp.cpp)
