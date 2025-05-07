cmake_minimum_required(VERSION 3.9)

project(bpa)

set(CMAKE_CXX_STANDARD 20)

file(GLOB_RECURSE SOURCE src/*)

add_library(bpa STATIC ${SOURCE})

target_include_directories(bpa PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/src
)