cmake_minimum_required(VERSION 3.15)
project(sort)

# 搜索源文件
aux_source_directory(${PROJECT_SOURCE_DIR} SRC)
# 或者用
# aux_source_directory(./ SRC)

# 头文件路径
include_directories(${HEADPATH})
# 指定静态库生成的目录
set(LIBRARY_OUTPUT_PATH ${LIBPATH})
add_library(${SORTLIB} STATIC ${SRC})