# 函数 
```/*
 swift中定义函数的格式 
 
 func 函数名称（参数列表）-> 返回值 
 {
    执行代码
 }
*/
```

## 函数四种类型
```// 1 类型1 没有返回值 没有参数
func sayHi()->Void
{
	print("hello type1");
}


//2 类型2 没有返回值 有参数
func say2(str:String)->Void{
	print(str);
}

//3 有返回值 没有参数
func say3()->String
{
	return "it is me";
}

//4 有返回值 有参数
func say4(str:String)->String
{
	return str;
}

```