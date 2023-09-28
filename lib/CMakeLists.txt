
# Create "test" Static Library 
#
# https://cmake.org/cmake/help/latest/command/add_library.html
#
# add_library(<name> [STATIC | SHARED | MODULE]
#             [EXCLUDE_FROM_ALL]
#             [<source>...])
add_library(test STATIC test.cpp)

# Header file path to use for library compilation 
target_include_directories(test PUBLIC ${CMAKE_SOURCE_DIR}/includes)

# Library Compile Options -Wall(Show all warnings), 
#                 -Werror(Warnings are considered compilation errors.)
target_compile_options(test PRIVATE -Wall -Werror)