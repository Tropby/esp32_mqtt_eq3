# The following lines of boilerplate have to be in your project's CMakeLists
# in this exact order for cmake to work correctly
cmake_minimum_required(VERSION 3.5)

include($ENV{IDF_PATH}/tools/cmake/project.cmake)

set(EXTRA_COMPONENT_DIRS components/mongoose)
include_directories(components/mongoose)
add_definitions(-DMG_ARCH=3)

project(esp32_mqtt_eq3)
