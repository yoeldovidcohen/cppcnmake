cmake_minimum_required(VERSION 3.17.3)
project(cppcnmake)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(main main.cpp)
target_link_libraries(main ${CONAN_LIBS})
