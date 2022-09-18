cmake_minimum_required(VERSION 3.4) #минимально требуемая версия для для сборки CMake
project(formatter) # название проекта

set(CMAKE_CXX_STANDARD 11) # установка стандартов
set(CMAKE_CXX_STANDARD_REQUIRED ON) # установка стандартов

add_library(formatter STATIC formatter.cpp formatter.h)

#target_include_directories(formatter PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
