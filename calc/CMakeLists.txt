cmake_minimum_required(VERSION 3.15)
project(calc)

# 搜索源文件
aux_source_directory(${PROJECT_SOURCE_DIR} SRC)
# 或者用
# aux_source_directory(./ SRC)

# 头文件路径
include_directories(${HEADPATH})
# 指定静态库生成的目录，注意这里是给宏赋值，所以不用${}，如果是取值的话需要
set(LIBRARY_OUTPUT_PATH ${LIBPATH})
add_library(${CALCLIB} STATIC ${SRC})