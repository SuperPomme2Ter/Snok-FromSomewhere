cmake_minimum_required(VERSION 4.3)
project(Snok_FromSomewhere)

set(CMAKE_CXX_STANDARD 20)

add_executable(Snok_FromSomewhere main.cpp)

find_package(SFML COMPONENTS Network Graphics Window Audio System CONFIG REQUIRED)
target_link_libraries(Snok_FromSomewhere PRIVATE SFML::Network SFML::Graphics SFML::Window SFML::Audio SFML::System)
