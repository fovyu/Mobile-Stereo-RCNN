cmake_minimum_required (VERSION 2.6)
project(eval_tool)

find_package(Boost REQUIRED COMPONENTS system)

include_directories(${Boost_INCLUDE_DIR})

add_executable(evaluate_object evaluate_object.cpp)

target_link_libraries(evaluate_object LINK_PUBLIC ${Boost_LIBRARIES})
