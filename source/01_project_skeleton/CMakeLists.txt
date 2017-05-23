cmake_minimum_required(VERSION 3.7)
project(01_project_skeleton)

set(CMAKE_CXX_STANDARD 11)

# Find includes in corresponding build directories
set(CMAKE_INCLUDE_CURRENT_DIR ON)
# Instruct CMake to run moc automatically when needed.
set(CMAKE_AUTOMOC ON)

set(SOURCE_FILES
        source/Shader.h
        source/Shader.cpp
        source/Program.h
        source/Program.cpp
        source/main.cpp)

add_executable(01_project_skeleton ${SOURCE_FILES})
target_link_libraries(01_project_skeleton GL GLU glut glfw GLEW)