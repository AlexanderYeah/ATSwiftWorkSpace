# 字符串
```
var str = "Hello, playground"


// 1 创建字符串
// 1.1 直接赋值
var str1 = "Hello World";
print(str1);
// 1.2 实例化方式
var str2 = String("This is me");
print(str2);

// 2 isEmpty 是否为空
var str3 = "";
print(str3.isEmpty);

// 3 字符串常量 使用let 修饰是不可变的 var 是可以变的
let str4 = "1123"; // 是不可变的
var str5 = "222"; // 是可以变的

// 4 字符串中插入值
var str6 = "great";
var val7:Float = 20.0;
var str8 = "";
str8 = "there are \(val7) person in this \(str6) country";
print(str8);

// 5 字符串的拼接
var str9 = "you are ";
var str10 = "so handsome";
var str11 = str9 + str10;
print(str11);

// 6 字符串的长度 count
var str12 = "give me the reason why are u stupid";
print(str12.count);

// 7 字符串比较
var str13 = "oc";
var str14 = "swift";
if str13 == str14{
	print("相等");
}else{
	print("不相等");
}

// 8 转换字符串数字为整形
let str15 = "123456";
let intStr:Int = Int(str15);





// 字符串的函数
// hasPrefix 是否拥有特定的前缀
// hasSuffix 是否有特定的后缀


```