cmake_minimum_required(VERSION 3.14)

project(Utils)

add_library(Utils STATIC)

target_sources(Utils
PRIVATE
    include/Utils/EventArena.hpp
    include/Utils/FileWatcher.hpp
    src/Resource.cpp
    include/Utils/Resource.hpp
    include/Utils/ResourceSettings.hpp
    include/Utils/ThreadPool.hpp
    include/Utils/type_list.hpp
)

target_include_directories(Utils
PUBLIC
    include
PRIVATE
    include/Utils
)
