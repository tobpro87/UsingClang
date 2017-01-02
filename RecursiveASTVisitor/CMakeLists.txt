set(SOURCE_FILES main.cpp)
add_executable(find-class-decls ${SOURCE_FILES})
target_link_libraries(find-class-decls clangTooling)
