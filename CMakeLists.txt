cmake_minimum_required(VERSION 3.22)
include(FetchContent)

project(CPPPackages)

add_compile_options(-std=c++17 -Wall)
add_link_options(-lstdc++ -lm)

FetchContent_Declare(
  googletest
  GIT_REPOSITORY https://github.com/google/googletest.git
  GIT_TAG release-1.12.1)
FetchContent_MakeAvailable(googletest)
