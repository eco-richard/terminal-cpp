
cmake_minimum_required(VERSION 3.21)

project(terminal-cpp)

set(CURSES_NEED_NCURSES TRUE)

find_package(Curses REQUIRED) 

add_executable(main main.cpp)

# target_include_directories(main ${CURSES_INCLUDE_DIRS})

# target_compile_options(main ${CURSES_CFLAGS})

target_link_libraries(main
PRIVATE
${CURSES_LIBRARIES})
