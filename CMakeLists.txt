cmake_minimum_required(VERSION 3.23)
project(cpp2tests VERSION 0.1.0 LANGUAGES C CXX)

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/cppfront)

find_package(fmt REQUIRED)

add_executable(cpp2tests main.cpp2)

target_link_libraries(cpp2tests PUBLIC fmt::fmt)
