add_executable(main "main.cpp")
target_include_directories(main external)
include(external/Catch)
catch_discover_tests(main)
