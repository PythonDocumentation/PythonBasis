# python集合

## 分类

可变类型元组set()

不可变类型元组frozenset()



## 函数

### `class set([iterable])`

### `class frozenset([iterable])`

构造一个元组类型
另外可以用 { } 构造一个元组

### `len(s)`

返回集合中元素的数量

### `x in s`

判断 x 在 s 内

### `x not in s`

判断 x 不在 s 内

### `s. isdisjoint(other)`

判断集合是不是相交，如果两集合有相同元素，则返回 True。

### `s. issubset(other)`

判断集合 s 是否在集合 other 中

### `s. issuperset(other)`

判断 other 是否被 s 包含

### `s. union(*others)`

### `set | other | ...`

求并集

### `s. intersection(*others)`

### `set & other & ...`

求交集，返回新集合

### `s. difference(*others)`

### `set - other - ...`

返回 集合*others 的补集

### `s. symmetric_difference(other)`

### `set ^ other`

对称差集，返回在 s 中但不在 other 中，或者在 other 中但不在 s 中的元素。

### `s. copy()`

用s的浅拷贝返回一个新的集合。

### `s. update(*others)`

### `set |= other | ...`

将集合 *others 中的元素添加到 s 中。

### `s. intersection_update(*others)`

### `set &= other & ...`

求并集，在原集合的基础上进行更改

### `s. difference_update(*others)`

### `set -= other | ...`

更新集合，移除 s 集合与 *others 的 并集。

### `s. add(elem)`

在集合 s 中添加元素 elem

### `s. remove(elem)`

去除 s 中的 elem 元素，如果没有则引发错误。

### `s. discard(elem)`

如果 s 中存在元素 elem 则