
cmake_minimum_required(VERSION 3.14...3.26)
project(
  book-word-counter
  VERSION 1.0
  DESCRIPTION "An application to extract and analyze most used words of ebooks"
  LANGUAGES CXX)

add_subdirectory(src)
add_subdirectory(apps)
set(CMAKE_CXX_STANDARD 17)
