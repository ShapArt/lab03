cmake_minimum_required(VERSION 3.4)
project(solver)

set(CMAKE_CXX_STANDARD 11) # установка стандартов
set(CMAKE_CXX_STANDARD_REQUIRED ON) # установка стандартов
add_executable(solve equation.cpp)
target_include_directories(solve PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib)
target_include_directories(solve PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/../solver_lib)
target_link_libraries(solve formatter_ex)
target_link_libraries(solve solver)
