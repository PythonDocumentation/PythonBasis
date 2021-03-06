# Python3 列表 list

## python的列表定义

列表定义时用 中括号 “[ ]”；

可以同时存储多种不同的数据类型；

类似于C语言中的数组；


## python的矩阵

python中矩阵可以用双层列表表示

## class list([iterable])

列表的构造

1. 使用一对方括号构造空列表：[ ]

2. 使用方括号，每个元素用逗号分隔：[a], [a, b, c]

3. 使用列表解析(迭代器生成)：[迭代器]

4. 使用对象的构造函数：list()

## Python列表脚本操作符

| 操作符格式 | 结果 | 含义 |

| len([1, 2, 3])                          | 3                            | 长度                       |
| --------------------------------------- | ---------------------------- | -------------------------- |
| [1, 2, 3] + [4, 5, 6]                   | [1, 2, 3, 4, 5, 6]           | 组合(两边是相同类型的序列) |
| ['Hi!'] * 4                             | ['Hi!', 'Hi!', 'Hi!', 'Hi!'] | 重复                       |
| 3 in [1, 2, 3]                          | True                         | 元素是否存在于列表中       |
| for x in [1, 2, 3]: print(x, end="   ") | 1 2 3                        | 迭代                       |

 

## Python列表截取与拼接

| L[2]  | 'Taobao'             | 索引 读取第三个元素                                       |
| ----- | -------------------- | --------------------------------------------------------- |
| L[-2] | 'Runoob'             | 索引 从右侧开始读取倒数第二个元素: count from the   right |
| L[1:] | ['Runoob', 'Taobao'] | 分片 输出从第二个元素开始后的所有元素                     |

 

## Python列表函数&方法

Python包含以下函数:

| len(list) | 列表元素个数       |
| --------- | ------------------ |
| max(list) | 返回列表元素最大值 |
| min(list) | 返回列表元素最小值 |
| list(seq) | 将元组转换为列表   |

 

## Python包含以下方法:

| list.append(obj)        | 在列表末尾添加新的单一对象                                   |
| ----------------------- | ------------------------------------------------------------ |
| list.clear()            | 清空列表                                                     |
| list.copy()             | 复制列表                                                     |
| list.count(obj)         | 统计某个元素在列表中出现的次数                               |
| list.extend(seq)        | 在列表末尾一次性追加另一个序列中的多个值（用新列表扩展原来的列表） |
| list.index(obj)         | 从列表中找出某个值第一个匹配项的索引位置                     |
| list.insert(index, obj) | 将对象插入列表固定位置index                                  |
| list.pop(obj=list[-1])  | 移除列表中的一个元素（默认最后一个元素），并且返回该元素的值 |
| list.remove(obj)        | 移除列表中某个值的第一个匹配项                               |
| list.reverse()          | 反向列表中元素                                               |
| list.sort([func])       | 对原列表进行排序                                             |

 