cmake_minimum_required(VERSION 3.0.0)
project(OSMKGP VERSION 0.1.0)

include(CTest)
enable_testing()

include_directories(${PROJECT_SOURCE_DIR}/libs/rapidxml)
include_directories(${PROJECT_SOURCE_DIR}/models)
include_directories(${PROJECT_SOURCE_DIR})

add_executable(OSMKGP main.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
