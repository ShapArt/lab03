cmake_minimum_required(VERSION 3.4) #минимально требуемая версия для для сборки CMake
project(formatter_ex) # название проекта

set(CMAKE_CXX_STANDARD 11) # установка стандартов
set(CMAKE_CXX_STANDARD_REQUIRED ON) # установка стандартов

add_library(formatter_ex STATIC formatter_ex.cpp formatter_ex.h) # сборка библиотеки

target_include_directories(formatter_ex PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/../formatter_lib)

target_link_libraries(formatter_ex formatter)
