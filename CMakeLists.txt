cmake_minimum_required(VERSION 3.27)
project(CGlions)
set(CMAKE_CXX_STANDARD 20)

find_package(OpenGL REQUIRED)

add_executable(CGlions src/main.cpp include/glad.h src/glad.c)

target_link_libraries(CGlions glfw OpenGL::GL)