cmake_minimum_required(VERSION 3.11)
project(lang)

add_subdirectory(3rd-party)
add_executable(main main.cpp)
add_executable(tests tests.cpp)

target_link_libraries(tests gtest)
