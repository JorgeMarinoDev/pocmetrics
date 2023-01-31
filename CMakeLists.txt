cmake_minimum_required(VERSION 3.20 FATAL_ERROR)

# Set c++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Project settings
project(poc-metrics
    VERSION 0.1
    LANGUAGES CXX
)

# Project folder structure
set(POCMETRICS_BIN_DIR ${PROJECT_SOURCE_DIR}/bin)
set(POCMETRICS_SOURCE_DIR ${PROJECT_SOURCE_DIR}/source)

####################################################################################################
# Targets
####################################################################################################
# Build main
add_executable(main ${POCMETRICS_SOURCE_DIR}/main.cpp)

# target_include_directories(main
#     PRIVATE
#     ${CLI11_SOURCE_DIR}/include
# )

#add_subdirectory(${ENGINE_SOURCE_DIR}/api)


#target_link_libraries(main base cmds api)

