Using Clang as a Library
=============================

## Preface
Please look at in the [Clang documentation](http://clang.llvm.org/docs/index.html) as a reference.

## Building

### Requirements
 - [LLVM 3.9.0](http://llvm.org/releases/download.html)+ (for libClang)
 - A C++11 compliant compiler

### Build

*Create a build directory.*

    mkdir build && cd build

*Export required environment variables*

	export LLVM_DIR=<path-to-clang-and-llvm-3.9.0>/lib/cmake/llvm
	export Clang_DIR=<path-to-clang-and-llvm-3.9.0>/lib/cmake/clang
   
*Generate a build system using any [desired generator](https://cmake.org/cmake/help/v3.0/manual/cmake-generators.7.html) in CMake. e.g "Unix Makefiles"*

    cmake -G "Unix Makefiles" ../
    
*Build - you can use any IDE if applicable to the generator, but you can also just build straight from CMake.*

    cmake --build .

## Provided Examples

[RecursiveASTVisitor based ASTFrontendActions](./RecursiveASTVisitor)


