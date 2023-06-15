cmake_minimum_required(VERSION 3.8)

project (Program)

set(SOURCE_FILES src/HotelManagmentSystem.cpp)

add_executable(Program ${SOURCE_FILES})

target_include_directories(Program PUBLIC include)