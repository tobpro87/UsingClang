set(SOURCE_FILES main.cpp)
add_executable(ASTMatchterLoopPrinter ${SOURCE_FILES})
target_link_libraries(
    ASTMatchterLoopPrinter
    clangTooling
    clangBasic
    clangASTMatchers
)
