cmake_minimum_required(VERSION 3.1)
project(mplite VERSION 0.0 LANGUAGES C)

set(CMAKE_C_STANDARD 90)
set(CMAKE_C_STANDARD_REQUIRED TRUE)
set(CMAKE_C_EXTENSIONS FALSE)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/inc/)

add_library(mplite src/mplite.c)
#target_include_directories(mplite PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/inc/)

add_executable(mplite_test
        src/mplite.c
        test/test.c)



