cmake_minimum_required(VERSION 2.8)
project(qwt)


find_package(Qt4 REQUIRED QtCore QtGui QtSvg QtXml)
include(${QT_USE_FILE})
add_definitions(${QT_DEFINITIONS})

add_subdirectory(src)
add_subdirectory(examples)
add_subdirectory(textengines)


