cmake_minimum_required(VERSION 3.13.4)
project(myProgram)

include_directories(include)

file(GLOB SOURCES "src/*.cpp")

add_executable(${PROJECT_NAME} ${SOURCES})
