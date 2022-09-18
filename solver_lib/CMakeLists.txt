cmake_minimum_required(VERSION 3.4)
project(solver)

set(CMAKE_CXX_STANDARD 20) # установка стандартов
set(CMAKE_CXX_STANDARD_REQUIRED ON) # установка стандартов

add_library(solver STATIC solver.cpp solver.h)
