cmake_minimum_required(VERSION 3.1)

# Project
project(ProgressBar)
find_package(Qt5Widgets CONFIG REQUIRED)

# Options
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Application
add_executable(ProgressBar WIN32 MACOSX_BUNDLE src/ProgressBar.cpp)
target_link_libraries(ProgressBar Qt5::Widgets)
