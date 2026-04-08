cmake_minimum_required(VERSION 3.10)
project(MemoryRiver)

set(CMAKE_CXX_STANDARD 17)

file(GLOB SOURCES "*.cpp")
if(NOT SOURCES)
    file(WRITE main.cpp "int main() { return 0; }")
    set(SOURCES main.cpp)
endif()

add_executable(code ${SOURCES})
