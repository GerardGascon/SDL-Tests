cmake_minimum_required(VERSION 3.24)
project(SDL_Tests)

set(CMAKE_CXX_STANDARD 17)

set(SDL2_INCLUDE_DIR C:/SDL2/include)
set(SDL2_LIB_DIR C:/SDL2/lib/x64)

include_directories(${SDL2_INCLUDE_DIR})
link_directories(${SDL2_LIB_DIR})

add_executable(SDL_Tests main.cpp)

target_link_libraries(${PROJECT_NAME} SDL2main SDL2)
