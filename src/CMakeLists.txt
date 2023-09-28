set(TARGET CMake_Example)

ADD_EXECUTABLE(${TARGET}  ${TARGET}.cpp)

target_compile_options(${TARGET} PRIVATE -Wall -Werror)

target_link_libraries(${TARGET} example)

set_target_properties(${TARGET} PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)