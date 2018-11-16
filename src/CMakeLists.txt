project( RigidBody )
cmake_minimum_required(VERSION 2.8)

# Enable C++ 2011 support
set(CMAKE_CXX_STANDARD 11)

# Enable multithreading
set(CMAKE_CXX_FLAGS ${CMAKE_CXX_FLAGS} "-std=c++11 -pthread")
set(CMAKE_CXX_IMPLICIT_LINK_DIRECTORIES /usr/local/lib ${CMAKE_CXX_IMPLICIT_LINK_DIRECTORIES})

# ----- Code directories:
# INCLUDE_DIRECTORIES( "rigidBody" )
# ADD_SUBDIRECTORY(    "RigidBody" )

# ----- tests directory
INCLUDE_DIRECTORIES( "tests" )
ADD_SUBDIRECTORY   ( "tests" )




