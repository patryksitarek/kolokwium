cmake_minimum_required(VERSION "3.10.2")

project(myProgram)

include_directories(include)

add_library(LibTest STATIC src/libtest.cpp)

add_executable(${PROJECT_NAME} src/Student.cpp)

target_link_libraries(${PROJECT_NAME} LibTest)

install(TARGETS ${PROJECT_NAME} DESTINATION bin)
install(FILES src/libtest.cpp DESTINATION lib)

