# 类的构造函数

* 类似于OC中的初始化方法 init
* 创建一个类，必然会调用一个构造函数
* 即便没有编写任何构造函数，编译器会提供一个默认的构造函数
* 继承自NSObject，可以对父类的构造函数进行重写

##  1 构造函数的基本使用 
```
class Person: NSObject {
	var name:String
	var age:Int
	override init() {
		name = "Alexander";
		age = 0;
	}
}


let p = Person();
```

## 2 初始化给属性赋值
* 很多时候，在创建一个对象的时候就会给属性赋值
* 可以自定义构造函数
* 如果定义了构造函数，会覆盖init方法，不在有默认的构造函数

```class Person: NSObject {
	var name:String
	var age:Int
	// 自定义构造函数 覆盖掉父类的函数
	init(name : String,age : Int){
		self.name = name;
		self.age = age;
	}
}


let p = Person(name: "alex", age: 15);

print(p.age);
```
### 3 字典转模型
* 真实创建对象时候,更多是将字典转成模型
* 在字典中取出的是NSObject任意类型，可以通过as！转成需要的类型，再进行赋值

```class Person: NSObject {
	
	var name : String;
	var age : Int;
	// 自定义构造函数 覆盖掉父类的函数
	init(dict : [String : NSObject]){
		name = dict["name"] as! String;
		age = dict["age"] as! Int;
	}
}

// 强制转换为需要的类型
let dict = ["name" : "alexander", "age" : 18] as! [String : NSObject];

let p = Person(dict: dict);

print(p.age);
```