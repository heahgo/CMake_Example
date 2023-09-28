add_library(test STATIC test.cpp)

target_include_directories(test PUBLIC ${CMAKE_SOURCE_DIR}/includes)

target_compile_options(test PRIVATE -Wall -Werror)