# OpenGL Project Template using CMake
A minimal C++ OpenGL project template using CMake to quickly get a project started.

## Features
- Cross-platform CMake build system
- GLFW for window and input handling
- GLAD for OpenGL function loading
- Basic window generation and rendering loop

## Prerequisites
- CMake
- A C++ compiler with C++11 support
- Git

## Building
When making changes to the files remember to rebuild the project before running again.
### Using Bash Scripts
``` bash
git clone https://github.com/SambaPro/OpenGL_Project_Template.git
cd OpenGL_Project_Template
./configure.sh
./build.sh
./run.sh
```

### Using Terminal
```
git clone https://github.com/SambaPro/OpenGL_Project_Template.git
cd OpenGL_Project_Template
mkdir build
cmake -B build -S src
cmake --build .
./my_project.exe
