project(snake_xenzia)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -std=c99")
set(SOURCE_FILES main.c game.c game.h ui_ncurses.c ui_ncurses.h)
add_executable(snake_xenzia ${SOURCE_FILES})

target_link_libraries(snake_xenzia ncurses)
target_link_libraries(snake_xenzia pthread)