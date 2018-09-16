cmake_minimum_required (VERSION 3.5)
project (MOBILENET_READ)


set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Ofast")


# Find libraries
set (CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake/")
message(${CMAKE_MODULE_PATH})

#find_package(FlatBuffers REQUIRED)
message(${FLATBUFF_INCLUDE})
include_directories(${FLATBUFF_INCLUDE})
include_directories(include)

add_subdirectory(src)





