set(HEADER_LIST ${book-word-counter_SOURCE_DIR}/include/ePubReader.hpp ${book-word-counter_SOURCE_DIR}/include/analyzer.hpp)
add_library(ePub_library ePubReader.cpp ${HEADER_LIST})
add_library(analyzer_library analyzer.cpp ${HEADER_LIST})
target_include_directories(ePub_library PUBLIC ../include)
target_include_directories(analyzer_library PUBLIC ../include)


source_group(
  TREE "${PROJECT_SOURCE_DIR}/include"
  PREFIX "Header Files"
  FILES ${HEADER_LIST})
