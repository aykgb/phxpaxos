# ut
aux_source_directory("${CMAKE_CURRENT_LIST_DIR}" UT_SOURCES)
message(STATUS "[LOG/ut] UT_SOURCES: ${UT_SOURCES}")
add_executable(ut ${UT_SOURCES})
target_link_libraries(ut ${CMAKE_BINARY_DIR}/src/libphxpaxos.a)
