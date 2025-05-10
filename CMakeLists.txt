cmake_minimum_required(VERSION 3.16)

set(VERSION 1.0.0)
set(PROJECT_NAME "VideoPlayer")
set(PROJECT_DESCRIPTION "A simple video player using Qt6")
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(${PROJECT_NAME} VERSION ${VERSION} LANGUAGES CXX)

find_package(Qt6 6.2 COMPONENTS Quick Gui REQUIRED)

qt_add_executable(${PROJECT_NAME}
    src/main.cpp
    src/qml/resources.qrc
)

target_link_libraries(${PROJECT_NAME} PRIVATE Qt6::Gui Qt6::Quick)