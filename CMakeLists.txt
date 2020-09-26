cmake_minimum_required(VERSION 3.17)
project(RayCastingInC)
set(CMAKE_CXX_STANDARD 14)

set(CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR}/cmake)
find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIR})

add_executable(${PROJECT_NAME} src/Main.c src/Constants.h)
target_link_libraries(${PROJECT_NAME} ${SDL2_LIBRARY})


