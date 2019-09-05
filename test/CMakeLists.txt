add_executable(main "main.cpp")
target_include_directories(main PUBLIC external)
include(external/Catch.cmake)
catch_discover_tests(main)
