cmake_minimum_required(VERSION 3.20)
project(blender2)

set(CMAKE_CXX_STANDARD 14)

add_executable(blender2 main.cpp)
find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)
include_directories(${OPENGL_INCLUDE_DIRS}  ${GLUT_INCLUDE_DIRS})
target_link_libraries(blender2 ${OPENGL_LIBRARIES}  ${GLUT_LIBRARY})


