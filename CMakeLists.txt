cmake_minimum_required(VERSION 3.22)

set(CMAKE_BUILD_TYPE "Debug")

project(CppProjectTemplate VERSION 1.0.0 LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD          20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS        OFF)

set(LIBRARY_NAME Library)
set(EXECUTABLE_NAME Executable)

add_subdirectory(src)
add_subdirectory(app)
add_subdirectory(configured)

#option(COMPILE_EXECUTABLE "Whether to compile the executable" OFF)
# if (COMPILE_EXECUTABLE)
#     add_subdirectory(app)
# endif()