cmake_minimum_required(VERSION 3.7)
project(05_asset_instance)

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
        source/tdogl/Camera.cpp
        source/tdogl/Camera.h
        source/main.cpp)

add_executable(05_asset_instance ${SOURCE_FILES})
target_link_libraries(05_asset_instance GL GLU glut glfw GLEW)