include_directories(include /usr/local/include)
FILE(GLOB src_files *.cpp)
add_library(implementation STATIC ${src_files} q_reg.cpp)
target_include_directories(implementation PUBLIC include /usr/local/include)
