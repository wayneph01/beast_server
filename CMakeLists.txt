cmake_minimum_required(VERSION 3.26)
project(BoostServer CXX)

set(BOOST_ROOT "/home/wayne/libs/boost")
Find_Package(Boost REQUIRED COMPONENTS headers)

add_executable (BoostServer
    advanced_server.cpp
)

target_link_libraries(BoostServer
    Boost::headers)
