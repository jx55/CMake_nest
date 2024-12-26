# CMake_nest
This is an example of how to use cmake nest.



这是一个演示CMake嵌套的例子。在每个目录中都编写了CMakeList.txt文件，然后根目录中有自己的CMakeLists.txt文件。大部分文件都是简单的演示文件，尤其是.cpp文件的内容并不重要。注意看文件的结构，与CMakeLists.txt的编写即可。



使用方法：

进入build目录：

`# 执行根目录中的CMakeLists.txt文件`

`cmake ../`

`make`



然后build的目录下会生成一系列文件，bin目录中会生成两个可执行文件，分别对应了test1和test2中的.cpp文件。
