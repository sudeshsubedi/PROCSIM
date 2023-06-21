cmake_minimum_required(VERSION 3.15)
project(PROCSIM)

set(CMAKE_CXX_STANDARD 11)


add_executable(PROCSIM 
    src/main.cpp
    src/process.cpp
    src/thread.cpp
    src/scheduler.cpp
    src/memoryblock.cpp
    src/memorymanager.cpp
)

target_include_directories(PROCSIM PRIVATE
    ${PROJECT_SOURCE_DIR}/include)

