cmake_minimum_required(VERSION 3.5)
project(my_project VERSION 3.5 LANGUAGES CXX)
add_executable(my_project main.cpp)
set_property(TARGET my_project PROPERTY CXX_STANDARD 20)

include(FetchContent)
include (CTest)
enable_testing()

# GLFW Fetch
FetchContent_Declare(
    glfw
    GIT_REPOSITORY https://github.com/glfw/glfw
    GIT_TAG "master"
    GIT_SHALLOW 1
)

FetchContent_MakeAvailable(glfw)


# Glad Fetch
FetchContent_Declare(
    glad
    GIT_REPOSITORY https://github.com/Sunday111/glad 
    GIT_TAG "main"
    GIT_SHALLOW 1
)

FetchContent_MakeAvailable(glad)

target_link_libraries(my_project PUBLIC glfw glad)