cmake_minimum_required(VERSION 3.14)

project(p1 CXX)

add_subdirectory(src)

option(BUILD_TESTING "Build tests" ON)

if(BUILD_TESTING)
  enable_testing()
  add_subdirectory(test)
endif()
