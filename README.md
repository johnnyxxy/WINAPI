# WINAPI.
\


windows相关api调用和实现便于使用的api
## GetProcessIDByName.cpp
通过进程名称查找进程id，返回的是所有符合名称要求的进程id列表。\
输出样例：\
编号    进程对应id(十六进制)    进程对应id(十进制)\
0       4314                    17172\
1       4314                    17172\
请按任意键继续. . .

## vmware虚拟机检测
该文件提供了一个用于检测当前运行环境是否为虚拟机的函数，通过读取对应端口的内容进行判断，若触发异常则运行环境不为vmware。


## usefunofexe
该文件夹提供了一种通过调试程序，使用程序中的某个功能的方法。提供了一个使用任何exe中任何函数的方法。
另一种使用其他应用程序的某项功能的例子见https://github.com/guanginuestc/AutoInput。

## debugmain
提供了多种在ring3环境下的反调试方案，其中函数可以直接使用，当进程处于被调试状态下时，反调试方案返回的均为1，否则为0.
## createremotethread
该文件夹下提供了一种使用远程线程进行dll注入的方案，并提供了样例dll的代码，当dll被成功注入的时候，会弹出对话框。

## InputMethodInjection
使用输入法注入技术对进程进行dll注入。其中ime.cpp为输入法源码，installime.cpp为输入法安装程序。
