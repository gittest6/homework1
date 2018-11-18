cmake_minimum_required(VERSION 3.9)

project(helloworld VERSION 1.$ENV{TRAVIS_BUILD_NUMBER})

add_executable(helloworld helloworld.cpp)

add_compile_definitions(TRAVIS_BUILD_NUMBER=$ENV{TRAVIS_BUILD_NUMBER})
