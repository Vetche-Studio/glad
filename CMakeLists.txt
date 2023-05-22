cmake_minimum_required(VERSION 3.20)

project(glad)

set(PROJECT_HEADERS 
    include/glad/glad.h
    include/KHR/khrplatform.h
)

set(PROJECT_SOURCES
    src/glad.c
)

add_library(${PROJECT_NAME} ${PROJECT_HEADERS} ${PROJECT_SOURCES})

target_include_directories(${PROJECT_NAME} PUBLIC include)