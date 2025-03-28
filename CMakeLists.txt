cmake_minimum_required(VERSION 3.14)
project(delusionml VERSION 0.1.0 LANGUAGES CXX OBJCXX)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Find required frameworks
find_library(METAL_LIBRARY Metal REQUIRED)
find_library(FOUNDATION_LIBRARY Foundation REQUIRED)

# Add includes
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)

# Add subdirectories as needed
add_subdirectory(src)

# Enable testing
#enable_testing()
#add_subdirectory(tests)