cmake_minimum_required(VERSION 3.24)

project(cppstarter LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(cppstarter
    src/main.cpp
)

target_include_directories(cppstarter PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)

if(MSVC)
    target_compile_options(cppstarter PRIVATE /W4 /permissive-)
else()
    target_compile_options(cppstarter PRIVATE -Wall -Wextra -Wpedantic)
endif()
