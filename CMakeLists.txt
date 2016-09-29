cmake_minimum_required(VERSION 3.3)

project(boost_throw_exception)

add_library(boost_throw_exception INTERFACE)

target_include_directories(boost_throw_exception BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_throw_exception DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
