set(TARGET main)

target_compile_options(test PRIVATE -Wall -Werror)

ADD_EXECUTABLE(${TARGET}  ${TARGET}.cpp)

target_link_libraries(${TARGET} test)

set_target_properties(${TARGET} PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)