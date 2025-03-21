cmake_minimum_required(VERSION 2.8.12...3.29)
project(sfp-c++)

set(CMAKE_CXX_STANDARD 11)

include_directories(../../src/include)
link_directories(../../build/debug/src)

add_executable(sfp select_from_parquet.cpp)
target_link_libraries(sfp duckdb)
