cmake_minimum_required(VERSION 3.10)
project(MiniVim)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# 收集 src 目录下的所有源文件
file(GLOB SOURCES "src/*.cpp")

# 生成可执行文件，名字必须是 code
add_executable(code ${SOURCES})
