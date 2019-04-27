cmake_minimum_required(VERSION 3.2)
project(liblmdb C)

file(GLOB_RECURSE SOURCE_FILES libraries/liblmdb/*.c)
file(GLOB_RECURSE HEADER_FILES libraries/liblmdb/*.h)

add_library(liblmdb ${SOURCE_FILES} ${HEADER_FILES})
include_directories(libraries/liblmdb)
