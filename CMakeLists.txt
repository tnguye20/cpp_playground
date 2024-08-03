cmake_minimum_required(VERSION 3.12)

project(playground)

set(CMAKE_CXX_STANDARD 20)

# Add your source files
set(SOURCES
    src/main.cpp
)
# Add your header files
set(HEADERS
    src/main.h
)

# Packages
# find_package(tl-expected CONFIG REQUIRED)

# Create an executable from your source files
add_executable(${PROJECT_NAME} ${SOURCES} ${HEADERS})

# Set the include directories
target_include_directories(${PROJECT_NAME}
    PRIVATE
    ${CMAKE_SOURCE_DIR}/include
)

# Set the include directories
target_include_directories(${PROJECT_NAME}
    PRIVATE
    ${CMAKE_SOURCE_DIR}/include
)

# target_link_libraries(${PROJECT_NAME} PRIVATE tl::expected)