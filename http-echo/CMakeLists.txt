cmake_minimum_required(VERSION 3.12)

project(hello)
add_subdirectory(poco)


add_executable(hello main.cpp)
target_link_libraries(hello PUBLIC Poco::Foundation Poco::Zip Poco::Net Poco::Util) # replace `...` by all poco library you use