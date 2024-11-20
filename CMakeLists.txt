cmake_minimum_required(VERSION 3.10)
project(MyLibrary)

set(CMAKE_C_STANDARD 99)

# Add source files to create a library
add_library(my_library
    src/add.c
    src/reduce.c
)

# Include directories for headers
target_include_directories(my_library PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)
