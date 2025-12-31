cmake_minimum_required(VERSION 3.29)

project(
        ECS_Project
        LANGUAGES
            CXX
)

add_executable(${CMAKE_PROJECT_NAME})

target_compile_features(${CMAKE_PROJECT_NAME} PRIVATE cxx_std_20)

target_include_directories(
        ${CMAKE_PROJECT_NAME}
            PRIVATE
                "include"
)

target_sources(
        ${CMAKE_PROJECT_NAME}
            PRIVATE
                "src/main.cpp"
                "include/foobar.h"
)
