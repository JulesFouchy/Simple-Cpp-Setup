cmake_minimum_required(VERSION 3.0)

# Set project name
project(SimpleCpp C CXX)
# Set C++ version
set(CXX_STANDARD 17)
# Set the folder where the executable is created
set(EXECUTABLE_OUTPUT_PATH 
    ${CMAKE_SOURCE_DIR}/bin/${CMAKE_BUILD_TYPE}
)

# Grab all the source files
file(GLOB_RECURSE MY_SOURCES
    src/*
)
# Create target executable
add_executable(${PROJECT_NAME}
    ${MY_SOURCES}
)
set_property(TARGET ${PROJECT_NAME} PROPERTY CXX_STANDARD ${CXX_STANDARD})

# Set include directories
include_directories(
    src
)

# Enable many good warnings
if(MSVC)
    target_compile_options(${PROJECT_NAME} PRIVATE /WX /W4)
else()
    target_compile_options(${PROJECT_NAME} PRIVATE -Werror -Wall -Wextra -Wpedantic -pedantic-errors -Wconversion -Wsign-conversion)
endif()