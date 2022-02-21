find_package(Pangolin REQUIRED)

set(CMAKE_CXX_FLAGS "-std=c++14")

find_package(OpenCV REQUIRED)

add_executable(stereoVision stereoVision.cpp)
target_link_libraries(stereoVision ${OpenCV_LIBS} ${Pangolin_LIBRARIES})
