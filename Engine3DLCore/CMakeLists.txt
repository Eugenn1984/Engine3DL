cmake_minimum_required(VERSION 3.28.1)

set(ENGINE_PROJECT_NAME Engine3DLCore)

add_library (${ENGINE_PROJECT_NAME} STATIC
	src/Engine3DLCore/Utils/test.cpp
	includes/Engine3DLCore/Utils/test.hpp
)

target_include_directories(${ENGINE_PROJECT_NAME} PUBLIC includes)
target_compile_features(${ENGINE_PROJECT_NAME} PUBLIC cxx_std_17)