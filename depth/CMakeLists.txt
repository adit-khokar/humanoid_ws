cmake_minimum_required(VERSION 2.8)
project( depth )
#set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/..)
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( exec depthf.cpp )
target_link_libraries( exec ${OpenCV_LIBS} )

