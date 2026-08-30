cmake_minimum_required(VERSION 3.20)
project(cs210_hello_world LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(cs210_hello_world src/main.cpp)

include(CTest)
if(BUILD_TESTING)
  add_test(NAME launches COMMAND cs210_hello_world)
endif()
