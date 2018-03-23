# 字典的使用
```// 4 字典数组
//4.1 创建字典的方式
//var dict = ["name":"alex","age":25];
//var val1 = dict["name"];
//print(val1!);

//4.2 创建字典的方式2 特定的键值Int 值的类型为String [keyType:valueType]()

var dict2 = [Int:String]();
dict2[1] = "alex";
dict2[2] = "jerry";
dict2[3] = "Alexander";
var val2 = dict2[1];

print(val2);


// 4.3 修改字典
dict2.updateValue("tom", forKey: 1);
var newval = dict2[1];
print(newval);


// 4.4 移除key-value 对
dict2.removeValue(forKey: 1);

print(dict2);

// 4.5 遍历字典
for(k,v) in dict2
{
	print("字典key \(k) 值value \(v)");
}


// 4.6 字典转换为数组
let dictKeys = dict2.keys;
let dictVals = dict2.values;

for k in dictKeys
{
	print(k);
}

for v in dictVals
{
	print(v);
}

// 4.7 计算count的属性
let count = dict2.count;

print(count);

// 4.8 isEmpty 属性 判断字典是否为空 返回的是布尔值 真为True 假为False
print(dict2.isEmpty);```