cmake_minimum_required(VERSION 3.15)

# set the project name and version
project(Tutorial VERSION 1.0)
list(APPEND CMAKE_PREFIX_PATH "~/pkg/libtorch_cpu_11/")

find_package(fcl REQUIRED)
find_package(Torch REQUIRED)

message(STATUS "CMAKE_MODULE_PATH:${CMAKE_MODULE_PATH}")
message(STATUS "CMAKE_CONFIG_PATH:${CMAKE_CONFIG_PATH}")
message(STATUS "CMAKE_PREFIX_PATH:${CMAKE_PREFIX_PATH}")

# The following variables are defined by cmake, notice the capital and lower case

message(STATUS "FCL_FOUND:${FCL_FOUND}")
message(STATUS "FCL_FOUND:${fcl_FOUND}")

message(STATUS "FCL_DIR:${fcl_DIR}")
message(STATUS "Torch_DIR:${Torch_DIR}")

message(STATUS "FCL_CONFIG:${FCL_CONFIG}")
message(STATUS "FCL_CONFIG:${fcl_CONFIG}")
message(STATUS "Torch_CONFIG:${Torch_CONFIG}")

# The following variables are defined by config.cmake files
message(STATUS "FCL_INCLUDE_DIRS:${FCL_INCLUDE_DIRS}")
message(STATUS "FCL_LIBRARIES:${FCL_LIBRARIES}")
message(STATUS "FCL_LIBRARY_DIRS:${FCL_LIBRARY_DIRS}")

message(STATUS "TORCH_INCLUDE_DIRS:${TORCH_INCLUDE_DIRS}")
message(STATUS "TORCH_LIBRARIES:${TORCH_LIBRARIES}")
message(STATUS "TORCH_LIBRARY_DIRS:${TORCH_LIBRARY_DIRS}")

message(STATUS "FCL_VERSION:${FCL_VERSION}")
message(STATUS "TORCH_VERSION:${TORCH_VERSION}")





