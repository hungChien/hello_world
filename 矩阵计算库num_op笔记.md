## copy库
1. copy.deepcopy():深度拷贝对象
2. 对于element为list的list对象,普通的切片索引复制并不是真正的拷贝,此时需要用到上面的方法
## python运算符重载
* python提供了很多运算符的重载,如下:
__add__,__radd__ | +
__iadd__ | +=
__sub__,__rsub__| -
__isub__ | -=
__len__ | len
__getitem__ | []
__setitem__ | a[i]=
__mul__, __rmul__ | *
__div__, __truediv__, __rdiv__ | /
__neg__ | -
__str__ | str()和print function
## slice对象
* 两个属性:slice.start和slice.stop
* slice对象指的是如(m:n)这样的切片,在重载__setitem__时常需要考虑slice
## 常用函数
1. isinstance(obj,(type1,type2...)):判断一个对象是否是某个类型
2. assert(....), "message":assert不符合时输出message信息
3. 双重列表解析与嵌套列表解析:
```Python
[n1 + n2 for n1,n2 in zip(lst1, lst2)] # 双重
[n1 + n2 for n1 in lst1 for n2 in lst2] # 嵌套
```
4. numpy数组转化为list:array.tolist()




