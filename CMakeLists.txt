cmake_minimum_required(VERSION 3.10)

project(imgui )

set(SOURCES
    ${CMAKE_CURRENT_SOURCE_DIR}/imgui.cpp
	${CMAKE_CURRENT_SOURCE_DIR}/imgui_demo.cpp
	${CMAKE_CURRENT_SOURCE_DIR}/imgui_draw.cpp
	${CMAKE_CURRENT_SOURCE_DIR}/imgui_tables.cpp
	${CMAKE_CURRENT_SOURCE_DIR}/imgui_widgets.cpp
)

add_library(imgui ${SOURCES})
target_include_directories(imgui PUBLIC 
	${CMAKE_CURRENT_SOURCE_DIR}/include/imgui
	${CMAKE_CURRENT_SOURCE_DIR}/
)
