add_executable(book-word-counter book-word-counter.cpp)
target_compile_features(book-word-counter PRIVATE cxx_std_17)
target_link_libraries(book-word-counter PRIVATE ePub_library analyzer_library)
