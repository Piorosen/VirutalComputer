SET(PROJ_NAME VirtualComputer)
project(${PROJ_NAME})
set(CMAKE_C_STANDARD                99)
set(CMAKE_CXX_STANDARD              14)
set(CMAKE_C_STANDARD_REQUIRED       ON)
set(CMAKE_CXX_STANDARD_REQUIRED     ON)
set(CMAKE_C_EXTENSIONS              OFF)
set(CMAKE_CXX_EXTENSIONS            OFF)

add_compile_definitions(MAX_MEMORY_SIZE=1024*4)
						

include_directories(${CMAKE_SOURCE_DIR}/inc)

add_executable(${PROJ_NAME} main.cpp)
