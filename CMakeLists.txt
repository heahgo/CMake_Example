CMAKE_MINIMUM_REQUIRED(VERSION 3.22.1)

PROJECT(
    CMake_Example
    DESCRIPTION "Cmake Exapmle"
    )

set(TARGET CMake_Example)        
set(OUTPUT_DIR ${CMAKE_SOURCE_DIR}/bin)

add_subdirectory(lib)
add_subdirectory(src)

