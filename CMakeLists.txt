project(foo)
cmake_minimum_required(VERSION 3.20.0)

enable_language(CXX CUDA)
find_package(CUDAToolkit)

add_executable(foo main.cpp foo.cu)
set_source_files_properties(foo.cu PROPERTIES LANGUAGE CUDA)
