# 类
### 一 类的定义 
  
可以继承自父类 也可以没有父类

class 类名:superClass {

}


```
class dog{
	var age:Int;
	init(age:Int) {
    self.age = age;
	}

}
```

### 类的属性
* 存储属性:存储实例的常量和变量   

* 计算属性: 并不存储实际的值,提供一个getter 和 可选的setter 来间接获取和设置其他属性.一般是只提供getter 

* 类属性: 类属性是与类相关联的，而不是与类的实例相关联，类属性的设置和修改，必须通过类来完成。使用Static 来修饰类属性


```
class Student {

	// 存储属性
	var age : Int = 0;
	var name : String!;
	var math : Int = 0;
	var phsic: Int = 0;
	// 计算属性 计算平均分
	var averageScore:Int{
		get {
			return ((math + phsic ) / 2);
		}
	
	}
	// 类属性
	static var grade:Int = 0;
	
}

let s = Student();
s.name = "alex";
s.math = 80;
s.phsic = 90;
// 类的属性必须通过类来设置
Student.grade = 2;
print(s.averageScore);
print(s.name);
```  




