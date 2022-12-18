# how c++ works

include

就是直接copy paste

x86 就是32



每个cpp都会生成.obj(windows) or .o(unix) 文件

link就会把这些文件拼接起来生成一个目标文件



# how compiling works

具体的在编译原理的仓库中

file does not mean anything

## 预处理

### include

编译中的include，就是复制粘贴

a.h

```
}
```

b.cpp

```
int a()
{
#include"a.h"
```

编译后程序正常执行

### define

就是简单的替换

### #if 

```
#if 1
...
#endif
```

...的部分就会编译否则不会



## **如果只是dbg，编译器不会优化**

## link

每个函数都会有一个签名，看起来就是随机数字



# 变量

```
char a = 56;//works
```



float 4bytes; double 8 bytes

```
//if we declare in this way
float a = 1.2;// auctually a will be a double value;
//so what we should do to declare a float 
float b = 12f;//add f or F at the end
```

![image-20221217183833660](img/image-20221217183833660.png)

为什么bool是一个byte不是一个bit

因为寻址问题 ，具体看计组或者os

sizeof 运算符 ，他不是函数



# function

最好减少函数调用，因为地址的跳转耗时



# Head file

```
#pragma once
```

```
#include<> 在include目录下 只用于编译器包含路径
#include"" 相对当前的
```





# debug

打断点，一步一步执行

step into: 进入到函数体内

step over: 从当前函数跳到下一行代码

step out: 跳出当前函数，回到调用这个函数的位置

在watch那里查看变量的类型和值

查看内存，&var

未初始化，为0xcccccccc

可以反汇编



# pointer

存储内存地址的整数







```
echo "# deep_of_c-" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:wuweipower/deep_of_c-.git
git push -u origin main
```

