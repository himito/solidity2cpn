# Specify the minimum version for CMake
cmake_minimum_required(VERSION 3.12.0)

# Project information
project(solidity2CPN CXX)

# C++11 required
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# installation folder
set(INSTALL_FOLDER ${PROJECT_SOURCE_DIR}/bin)

# Third-party libraries
add_subdirectory(third-party)

# Source folder
add_subdirectory(src)

# The executable code is here
add_subdirectory(app)

# documentation
add_subdirectory(docs)