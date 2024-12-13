cmake_minimum_required(VERSION 3.10)

project(BasicSpaceShooter VERSION 0.0.1
                  DESCRIPTION "A simple OpenGL game engine"
                  LANGUAGES CXX)

find_package(glfw3 CONFIG REQUIRED)
find_package(glad CONFIG REQUIRED)

add_executable(${PROJECT_NAME} main.cpp)

target_link_libraries(${PROJECT_NAME} PRIVATE glfw glad::glad)
