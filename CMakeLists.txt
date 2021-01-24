# cmake version to be used
cmake_minimum_required( VERSION 3.0 )

# project name
project( filesystem )

# include
include_directories( ./src )

find_package (Threads)

# target
add_executable( binary ./src/main.cpp ./src/human.cpp ./src/bot.cpp )

add_executable( test ./test/main.cpp ./src/human.cpp ./src/bot.cpp )


# target_link_libraries (server ${CMAKE_THREAD_LIBS_INIT})
