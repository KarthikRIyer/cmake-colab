cmake_minimum_required(VERSION 3.12 FATAL_ERROR)

project(cmake-colab VERSION 1.0.0 LANGUAGES CXX C)

set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_CXX_STANDARD 14)

# default to Release build
if (NOT CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE Release CACHE STRING
            "Choose the type of build, options are: None Debug Release RelWithDebInfo MinSizeRel."
            FORCE)
endif ()


add_executable(cmake-colab
        main.cpp)
