project(opensse)

cmake_minimum_required(VERSION 3.17)

find_package(OpenCV REQUIRED COMPONENTS opencv_core opencv_imgproc opencv_imgcodecs opencv_highgui opencv_features2d opencv_ml)
find_package(Threads REQUIRED)

include_directories(/usr/local/include)
include_directories(..)
include_directories(${PROJECT_SOURCE_DIR}/sse)

link_directories(/usr/local/lib)

add_subdirectory(sse)
add_subdirectory(tools)