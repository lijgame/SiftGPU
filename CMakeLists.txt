CMAKE_MINIMUM_REQUIRED(VERSION 3.16)
if(POLICY CMP0072)
  cmake_policy(SET CMP0072 NEW)
endif()

PROJECT(SIFTGPU C CXX)

SET(CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} -Wno-write-strings -Wno-unused-result -Wno-deprecated -fPIC")
SET(CMAKE_C_FLAGS  "${CMAKE_C_FLAGS} -Wno-write-strings -Wno-unused-result -Wno-deprecated -fPIC")

ADD_SUBDIRECTORY(src)

