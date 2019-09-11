# for 循环

for 循环在 Python 中是一个通用的迭代器：
可以遍历任何有序的序列对象内的元素

for 语句可用于字符串、列表、元组、其他内置可迭代对象以及之后我们能够用通过类所创建的新对象

当 Python 运行 for 循环时，会逐个将序列对象中的元素赋值个目标，然后为每个元素执行循环主体。

for 循环中也支持一个选用的 else块 ，当循环内部没有 break 跳出循环时，就会执行

## 一般格式

```python
for <target> in <object>:
	<statement>
else:
	<statement>
```

## 循环格式
```python
for <target> in <object>:
	<statements>
	if <test>: break
	if <test>: continue
else:
	<statements>
```

## for 循环的用法

```python
name = "laowang"
for temp in name:
    print("---")
    print(temp)
```

## for...else
### 列表字典

```python
card_infors = [
    {
        'name':'laowang',
        'age':18
    },
    {
        'name':'laoli',
        'age':19
    },
    {
        'name':'laozhao',
        'age':20
    }
]
```

### 输入要查询的名字

```python
find_name = input('请输入要查询的名字：')
```
### 遍历查找
```python
for temp in card_infors:
    if temp['name'] == find_name:# 如果找到
        print('找到人了。。。。')# 输出信息
        break# 跳出 for 循环
else:# 没有找到
    print('没有找到')# 输出信息
```

