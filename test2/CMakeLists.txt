cmake_minimum_required(VERSION 3.15)
project(test2)

aux_source_directory(./ SRC)
include_directories(${HEADPATH})

# 指定静态库的路径、链接静态库
link_directories(${LIBPATH})
link_libraries(${SORTLIB})
# 设置可执行文件生成的路径、生成可执行文件
set(EXECUTABLE_OUTPUT_PATH ${EXECPATH})
add_executable(${APPNAME2} ${SRC})