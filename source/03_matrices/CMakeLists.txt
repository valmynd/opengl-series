cmake_minimum_required(VERSION 3.7)
project(03_matrices)

set(CMAKE_CXX_STANDARD 11)

# Find includes in corresponding build directories
set(CMAKE_INCLUDE_CURRENT_DIR ON)
# Instruct CMake to run moc automatically when needed.
set(CMAKE_AUTOMOC ON)

set(SOURCE_FILES
        source/tdogl/stb_image.h
        source/tdogl/Bitmap.cpp
        source/tdogl/Bitmap.h
        source/tdogl/Program.cpp
        source/tdogl/Program.h
        source/tdogl/Shader.cpp
        source/tdogl/Shader.h
        source/tdogl/Texture.cpp
        source/tdogl/Texture.h
        source/main.cpp)

add_executable(03_matrices ${SOURCE_FILES})
target_link_libraries(03_matrices GL GLU glut glfw GLEW)