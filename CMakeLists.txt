cmake_minimum_required(VERSION 3.5.1)
project(UsingClang CXX)

find_package(Clang)

link_directories(${LLVM_LIBRARY_DIR})
include_directories(${LLVM_INCLUDE_DIRS})

add_definitions(${LLVM_DEFINITIONS})

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fno-rtti -std=c++11")

add_subdirectory(./RecursiveASTVisitor)
add_subdirectory(ASTMatcherLoopPrinter)




