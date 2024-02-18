cmake_minimum_required(VERSION 3.16)
project(gothic3sdk)

include(source/CMakeLists.txt)

target_link_directories(gothic3sdk PUBLIC lib)
target_link_libraries(gothic3sdk PUBLIC
    Engine
    Game
    GFC
    Importer
    Script
    SharedBase
)

target_compile_options(gothic3sdk PUBLIC /Gz)