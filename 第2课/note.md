# c++ lesson2

## 处理数据
------------
* C++变量的命名规则。
* C++内置的整型——unsigned long、long、unsigned int、int、unsigned short、short、char、unsigned char、signed char和bool。
* C++11新增的整型：unsigned long long和long long。
* 表示各种整型的系统限制的climits文件。
* 各种整型的数字字面值（常量）。
* 使用const限定符来创建符号常量。
* C++内置的浮点类型：float、double和long double。
* 表示各种浮点类型的系统限制的cfloat文件。
* 各种浮点类型的数字字面值。
* C++的算术运算符。
* 自动类型转换。
* 强制类型转换。

摘录来自: [美] Stephen Prata. “C++ Primer Plus（第6版）中文版。” Apple Books. 
----------------------

--------

### 1.1 简单变量

“程序通常都需要存储信息—如Google股票当前的价格、纽约市8月份的平均湿度、美国宪法中使用最多的字母及其相对使用频率或猫王模仿者的数目。为把信息存储在计算机中，程序必须记录3个基本属性：”


* 信息将存储在哪里；
* 要存储什么值；
* 存储何种类型的信息。

例:

```c++
int braincount;
braincount = 5;
```
“这些语句告诉程序，它正在存储整数，并使用名称braincount来表示该整数的值（这里为5）。实际上，程序将找到一块能够存储整数的内存，将该内存单元标记为braincount，并将5复制到该内存单元中；然后，您可在程序中使用braincount来访问该内存单元。这些语句没有告诉您，这个值将存储在内存的什么位置，但程序确实记录了这种信息。实际上，可以使用&运算符来检索braincount的内存地址。下一章介绍另一种标识数据的方法（使用指针）时，将介绍这个运算符。”


#### 1.1.1 变量名

> c++ “提倡使用有一定含义的变量名。如果变量表示差旅费，应将其命名为cost_of_trip或costOfTrip，而不要将其命名为x或cot。必须遵循几种简单的C++命名规则。”

* 名称的第一个字符不能是数字。
* 区分大写字符与小写字符。
* 不能将C++关键字用作名称。
* 以两个下划线或下划线和大写字母打头的名称被保留给实现（编译器及其使用的资源）使用。以一个下划线开头的名称被保留给实现，用作全局标识符。
* C++对于名称的长度没有限制，名称中所有的字符都有意义，但有些平台有长度限制。

摘录来自: [美] Stephen Prata. “C++ Primer Plus（第6版）中文版。” Apple Books. 

倒数第二点与前面几点有些不同，因为使用像_time_stop或_Donut这样的名称不会导致编译器错误，而会导致行为的不确定性。换句话说，不知道结果将是什么。不出现编译器错误的原因是，这样的名称不是非法的，但要留给实现使用。

下面使一些错误的c++变量名：

```c++
int poodle;
int my_asdasd;
int double;
int begain;
int __adsasd__;
int honey-hook;
```

“符 号 常 量

表 示

CHAR_BIT

char的位数

CHAR_MAX

char的最大值

CHAR_MIN

char的最小值

SCHAR_MAX

signed char的最大值

SCHAR_MIN

signed char的最小值”






