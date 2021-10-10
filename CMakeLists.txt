CMAKE_MINIMUM_REQUIRED(VERSION 2.8.12) #cmake最低版本需求，不加入此行会受到警告信息

PROJECT(Salsa20) #项目名称

AUX_SOURCE_DIRECTORY(./src SRC_LIST) #把当前目录(.)下所有源代码文件和头文件加入变量SRC_LIST
INCLUDE_DIRECTORIES(./include)
ADD_EXECUTABLE(main ${SRC_LIST}) #生成应用程序 main
