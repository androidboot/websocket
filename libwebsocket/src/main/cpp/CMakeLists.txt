cmake_minimum_required(VERSION 3.4.1)


add_library(websocket
        SHARED

        websocket-lib.cpp)

find_library(log-lib log)


target_link_libraries(
        websocket

        ${log-lib})