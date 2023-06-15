cmake_minimum_required(VERSION 3.8)

project(Library)

set(SOURCE_FILES src/model/Room.cpp src/model/Person.cpp)

add_library(Library ${SOURCE_FILES})

target_include_directories(Library PUBLIC include)