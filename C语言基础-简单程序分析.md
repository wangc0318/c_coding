## C语言基础-简单程序分析

在上一篇文章里介绍了C语言的入门程序HelloWorld，[入门程序HelloWorld][1]
在这一篇里我们继续来看C语言的入门程序，我们先来看一个简单的程序。

```c
#include<stdio.h>

int addFunc(int x,int y) {/*定义一个加法函数*/
    return x + y;/*返回两个数的和*/
}

int main() {
    int a, b, result;
    a = 2;
    b = 3;
    result = addFunc(a,b);/*调用addFunc()函数*/
    printf("%d+%d=%d\n",a,b,result);/*将结果打印*/
    return 0;
}
```
代码运行结果如下图所示：

![这里写图片描述](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9pbWctYmxvZy5jc2RuLm5ldC8yMDE4MDMxODIwMTgzMDk_d2F0ZXJtYXJrLzIvdGV4dC9MeTlpYkc5bkxtTnpaRzR1Ym1WMEwyTnpaRzVmZDJGdVoyTm9iMjVuL2ZvbnQvNWE2TDVMMlQvZm9udHNpemUvNDAwL2ZpbGwvSTBKQlFrRkNNQT09L2Rpc3NvbHZlLzcw?x-oss-process=image/format,png)

我们来分析一下这段代码的结构：
首先是一个`addFunc(int x,int y)`函数，这个函数的功能是计算两个数的和，并将和返回给主调函数main()。
`main()`里首先定义了三个变量，进而对a,b初始化。然后调用`addFunc()`函数，在调用`addFunc()`时，传入的参数是变量a和变量b，这两个参数称为实际参数（实参）。将实参a,b的值分别传给了`addFunc(int x,int y)`函数中的形式参数`x,y`，经过`addFunc()`函数的处理，将x,y相加的和的值（实际就是`a,b`相加和的值）赋给`result`变量。最后将结果通过`printf()`函数打印输出。
代码已经上传到github[传送门][2]

后面会持续更新C语言基础以及C语言进阶的一些内容，跟大家一起学习C语言。


[1]: https://blog.csdn.net/csdn_wangchong/article/details/79603824
[2]: https://github.com/wangchong0327/c_cpp_study_demo.git