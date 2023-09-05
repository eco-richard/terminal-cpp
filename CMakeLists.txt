
cmake_minimum_required(VERSION 3.21)

project(terminal-cpp)

find_package(ftxui CONFIG REQUIRED)

add_executable(main main.cpp)

target_link_libraries(main
PRIVATE
ftxui::dom
ftxui::screen
ftxui::component)

