cmake_minimum_required(VERSION 3.21)
project(DarkDash)

set(CMAKE_CXX_STANDARD 20)

add_library(${DarkDash} SHARED
    src/main.cpp
)

target_link_libraries(${DarkDash} Geode::Geode)

setup_geode_mod(${DarkDash})
