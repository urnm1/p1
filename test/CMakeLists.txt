add_executable(main "main.cpp")
target_include_directories(main PUBLIC external)
target_compile_options(main PRIVATE -O0 -g -fprofile-arcs --coverage)
target_link_libraries(main PRIVATE gcov)
include(external/Catch.cmake)
catch_discover_tests(main)
