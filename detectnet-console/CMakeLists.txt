
file(GLOB detectnetConsoleSources *.cpp)
file(GLOB detectnetConsoleIncludes *.h )

add_executable(detectnet-console ${detectnetConsoleSources})
target_link_libraries(detectnet-console nvcaffe_parser nvinfer jetson-inference)
