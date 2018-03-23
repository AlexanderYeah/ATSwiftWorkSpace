# 数组
```print("hello from other side");

// 1 构造数组的方式
// var array1 = [sometype]()
// var array2 = [someType](repeating:初始值;count:元素个数)
// var someInts:[Int] = [10,20,30];

// 2 访问数组 通过索引
var array1 = [Int](repeatElement(10, count: 4));

// 3 修改数组
// 3.1 append
array1.append(20);
print(array1);
// 3.2 或者使用 += 拼接 数组
array1 += [30];
print(array1);
// 3.3 使用索引修改
array1[3] = 90;
print(array1);


// 4 遍历数组
for item in array1
{
	print(item);
}

// 5 合并数组 就是相加 前提是两个数组类型相同
var array2 = [1,2,3,4];
var newArray =  array1 + array2;

print(newArray);

// count 属性 数组的数量
// isEmpty 数组是否为空


```