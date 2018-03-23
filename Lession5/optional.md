# Optional 可选类型
```// 可选类型
// Optional 类型 ,用来表示有值或者没有值
var str1:String? = "hello world";

// 强制解析 使用 ！ 进行强制解析
// 当确定str1 确实包含值之后，可以使用感叹号来获取值
if str1 != nil {
	print(str1!);
}

// 在声明变量的时候使用感叹号替换问号,在使用可选变量的时候就不用通过感叹号获取值
var str2:String! = "you got me";
if str2 != nil {
    print(str2);
}

// 可选绑定(optional banding) 来判断可选类型是否包含值,如果包含值，赋给一个临时常量或则变量
var str3:String? = nil;
if let str4 = str3 {
	print("你的可选类型str3 有值");
}else{
	print("你的可选类型str3 没有值");
}

```