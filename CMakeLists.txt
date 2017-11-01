cmake_minimum_required(VERSION 3.0)

project(april C)

get_filename_component(BASE_SRC_ROOT ${CMAKE_CURRENT_SOURCE_DIR}/src ABSOLUTE)
get_filename_component(BASE_INC_ROOT ${CMAKE_CURRENT_SOURCE_DIR}/include ABSOLUTE)

include_directories(${BASE_INC_ROOT})

add_subdirectory(${BASE_SRC_ROOT}/parser)

