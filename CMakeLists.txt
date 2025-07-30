cmake_minimum_required(VERSION 3.25)

project(Learn-vscode-cmake-project LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)

add_library(my_lib SHARED lib/my_lib.cpp)
target_include_directories(my_lib PUBLIC lib)

add_executable(main main.cpp)
target_link_libraries(main PRIVATE my_lib)
