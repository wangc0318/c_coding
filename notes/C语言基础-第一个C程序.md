## C语言基础-第一个C程序

之前在大学期间学过C语言的基础，后来主要方向是java，就没继续深入学习C语言。但是C语言作为一个基础语言，对开发有着很大的帮助。最近又开始用业余时间系统的学习C语言。

首先，简单的介绍一下C语言
**C语言是一种结构化，与机器无关且执行效率高的语言。**
### C语言的基本特点
* 简洁灵活
* 功能强大
* 可移植
* 语法灵活自由
* 标准库

### 第一个C程序
关于C语言的有点以及为什么我们要学习C语言这里就不多说了，下来我们直接进入今天的主题，编写第一个C程序。
和学习其它语言一样，先从Hello World开始
在此先说一下使用的编程工具，工具有好多种，这里使用的工具是VS2017，为什么使用VS就不用了我多说了吧。
首先打开工具，开打后直接快捷键Ctrl+shift+n 
![这里写图片描述](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9pbWctYmxvZy5jc2RuLm5ldC8yMDE4MDMxODIwMDY1NjcyNz93YXRlcm1hcmsvMi90ZXh0L0x5OWliRzluTG1OelpHNHVibVYwTDJOelpHNWZkMkZ1WjJOb2IyNW4vZm9udC81YTZMNUwyVC9mb250c2l6ZS80MDAvZmlsbC9JMEpCUWtGQ01BPT0vZGlzc29sdmUvNzA?x-oss-process=image/format,png)
选择 Empty Project，填上项目名称，点击OK，项目创建完成。
然后新建一个.c文件

然后输入一下代码

```c
#include<stdio.h>

int main() {                   /*主函数*/
    printf("hello world!\n");  /*输出hello world！*/
    return 0;                  /*返回*/
}
```
Ctrl+F5运行，运行结果如下：
![这里写图片描述](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9pbWctYmxvZy5jc2RuLm5ldC8yMDE4MDMxODIwMDg0NjQ1ND93YXRlcm1hcmsvMi90ZXh0L0x5OWliRzluTG1OelpHNHVibVYwTDJOelpHNWZkMkZ1WjJOb2IyNW4vZm9udC81YTZMNUwyVC9mb250c2l6ZS80MDAvZmlsbC9JMEpCUWtGQ01BPT0vZGlzc29sdmUvNzA?x-oss-process=image/format,png)
入门的第一个程序HelloWorld已经完成。
我们来分析一下上面这段代码：
`#include<stdio.h>`为文件包含命令，而`stdio.h`是头文件，它里面包含里一些程序中需要使用的基本元素，`printf()`就是其中一个。
下面定义了一个`main()`函数，int为函数的返回值类型，利用`printf()`函数输出了字符串`"hello world"`,而`"\n"`是换行符，它在这里的作用是输出`"hello world"`后换行。`return 0`表示返回。
代码中`"/*...*/"`是注释，它的内容不参与程序运行。C语言中单行注释也可以用`"\\"`。
下图总结了组成C程序的几个部分
![C程序解剖](https://img-blog.csdnimg.cn/20190309202651321.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NzZG5fd2FuZ2Nob25n,size_16,color_FFFFFF,t_70)
好了，第一个C程序就介绍到这里，这里再额外说一下**编程的7个步骤**，为了直观明了，直接奉上一张图
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191107213801977.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NzZG5fd2FuZ2Nob25n,size_16,color_FFFFFF,t_70)

github地址：https://github.com/wangchong0327/c_cpp_study_demo.git