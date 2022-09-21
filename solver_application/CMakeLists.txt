cmake_minimum_required(VERSION 3.4)
project(equation)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(equation equation.cpp)

target_include_directories(equation PUBLIC $(CMAKE_CURRENT_SOURCE_DIR)/../formatter_ex_lib)
target_include_directories(equation PUBLIC $(CMAKE_CURRENT_SOURCE_DIR)/../solver_lib)

target_link_libraries(equation formatter_ex)
target_link_libraries(equation solver)
