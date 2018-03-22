# Review Swift

一 特点 

* 快速，现代，安全，互动，而且明显优于Objective-C

* 取消了OC的指针以及其他不安全的访问的使用

* 舍弃OC早起应用的SmallTalk 的语法，全面改为句点表示法

* 提供了类似Java 的名字空间（namespace），泛型（generic），运算对象重载（operate overloading）

* Swift 被称为“没有C的Obective-C” 


```import UIKit

var str = "Hello, playground";
// 1  打印字符串
print (str);


// 2 常量的定义
// let 代表常量 不可变的
// var 代表变量
let num = 10.1;
var value  = 8;

value = 15;

// 3 逻辑分支
// 3.1 包头不包尾部
for i in 0..<10
{
	print(i);
}
// 3.2 包头也包尾
for i in 0...10
{
	print(i);
}
// 3.3 不关心某个参数 使用_
for _ in 0..<5
{
	print("132");
}


```