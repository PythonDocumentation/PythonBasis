# while 循环

while 循环中支持一个选用的 else块 ，当循环内部没有 break 跳出循环时，就会执行


while 循环必须有一个初始条件，及作为参数的变量必须在循环外进行定义
	循环必须有一个终止条件
	循环可以没有 else 语句

## 一般格式

```python
while <test>:
	<statrments1>
else:
	<statements2>

<test>: 测试表达式
<statments1>: 有一列或多列缩进语句的主体
else: 可选择的部分
```

## 一般循环格式

```python
while <test1>
	<statements1>
	if <test2>: break
	if <test3> continue
else:
	<statements2>
# break 和 continue 可以出现在 while（或for）循环的任何地方
```



## 打印 1 - 10 的数字

```python
num = 1
while num < 11:
    print(num,end="\n")
    num += 1
else:
    print("输出完毕") 
```
