# 闭包
## sorted 方法
swift 标准库提供了名为 sorted(by:) 的方法，会根据您提供的用于排序的闭包函数将已知类型数组中的值进行排序。
排序完成后，sorted(by:) 方法会返回一个与原数组大小相同，包含同类型元素且元素已正确排序的新数组。原数组不会被 sorted(by:) 方法修改。 
`
var arr1 = [3,8,13,66,22];


func showMax(val1:Int,val2:Int) -> Bool{
	return val1 > val2;
}

var newArr = arr1.sorted(by:showMax);
// 排序结果  [66, 22, 13, 8, 3]`
