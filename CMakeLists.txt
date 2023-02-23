# If you create new headers/cpp files, add them to these list!

#include_directories(inlude);
# set(HEADER_FILES
#     inlude/cpplib.h
# )
file(GLOB_RECURSE SOURCE_FILES "src/*.cpp")
# set(SOURCES
#     src/cpplib.cpp
# )
add_executable(cpplib main.cpp ${SOURCE_FILES})
target_include_directories(cpplib PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/include)