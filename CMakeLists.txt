cmake_minimum_required (VERSION 3.14)
project (Branches LANGUAGES CXX)

#please don't build Debug version on windows

set(CMAKE_CXX_STANDARD 20)
file(GLOB_RECURSE src_files CONFIGURE_DEPENDS "src/*.cpp" "src/*.hpp" "src/*.h")


add_executable(Branches ${src_files})