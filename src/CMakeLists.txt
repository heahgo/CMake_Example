set(TARGET CMake_Example)

target_compile_options(test PRIVATE -Wall -Werror)

ADD_EXECUTABLE(${TARGET}  ${TARGET}.cpp)

target_link_libraries(${TARGET} example)

set_target_properties(${TARGET} PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)