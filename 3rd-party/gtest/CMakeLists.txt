find_package(Threads REQUIRED)

add_library(gtest src/gtest-all.cc include/gtest/gtest.h)
target_include_directories(gtest PUBLIC include)
target_link_libraries(gtest Threads::Threads)
