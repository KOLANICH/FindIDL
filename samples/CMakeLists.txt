cmake_minimum_required(VERSION 3.8)

project(FindIDL LANGUAGES C CXX CSharp)
set_property(GLOBAL PROPERTY USE_FOLDERS ON)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/../cmake")
find_package(IDL REQUIRED)

set(MIDL_FLAGS /target NT60)

add_subdirectory(Demo)