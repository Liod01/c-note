# c++ 一些基础库，函数使用

------------
## cmath

###  [<cmath> (math.h) - C++ Reference](http://www.cplusplus.com/reference/cmath/)

函数原型之于函数就像变量声明之于变量—指出涉及的类型。例如，C++库将sqrt( )函数定义成将一个（可能）带小数部分的数字（如6.25）作为参数，并返回一个相同类型的数字。有些语言将这种数字称为实数，但是C++将这种类型称为double。sqrt( )的函数原型像这样：

``` c++
double sqrt(double);          //函数使用
```
``` c++
double x;
x = sqrt(6.25)
```
``` c++
#include <iostream>
#include <cmath>

using namespace std

int main(int argc, char const *argv[])
{
    double area;
    cout << "请输入你的double数" << ;
    cin >> area;
    double side;
    side = sqrt(area);
    cout << "area的值为: " << side << endl; 
    /* code */
    return 0;
}
```
使用例子

* 求数的几次方 
```c++
answer = pow(5.0, 8.0)
```


标准C库提供了140多个预定义的函数。如果其中的函数能满足要求，则应使用它们。但用户经常需要编写自己的函数，尤其是在设计类的时候。无论如何，设计自己的函数很有意思，下面来介绍这一过程。前面已经使用过好几个用户定义的函数，它们都叫main( )。每个C++程序都必须有一个main( )函数，用户必须对它进行定义。假设需要添加另一个用户定义的函数。和库函数一样，也可以通过函数名来调用用户定义的函数。对于库函数，在使用之前必须提供其原型，通常把原型放到main( )定义之前。但现在您必须提供新函数的源代码。最简单的方法是，将代码放在main( )的后面。

### Question ?

* c++ 程序的模块叫什么
*  #include ``<iostream>`` 有什么用
*  定义函数什么时候可以不使用return

![15458881409204.png](https://image.3001.net/images/20181227/15458881409204.png)

### 练习
1．编写一个C++程序，它显示您的姓名和地址。
2．编写一个C++程序，它要求用户输入一个以long为单位的距离，然后将它转换为码（一long等于220码）。
3．编写一个程序，让用户输入其年龄，然后显示该年龄包含多少个月，如下所示：
![226dac42a61ab7c207244de770dadf70.png-quanzi](http://secquan.zzyuncheng.com/226dac42a61ab7c207244de770dadf70.png-quanzi)


4．编写一个程序，要求用户输入小时数和分钟数。在main( )函数中，将这两个值传递给一个void函数，后者以下面这样的格式显示这两个值：
![db417dcd6426895f4edbb1a57b92323b.png-quanzi](http://secquan.zzyuncheng.com/db417dcd6426895f4edbb1a57b92323b.png-quanzi)


