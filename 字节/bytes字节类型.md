# 字节类型

二进制字节类型，不可变
只允许ASCII字符的字节数(不管声明的源代码编码)。任何大于127的二进制值都必须使用适当的转义序列输入字节。

### bytes.count(sub[, start[, end]])

### bytearray.count(sub[, start[, end]])

返回子序列sub在[start,end]中出现的次数

### bytes.decode(encoding="utf-8", errors="strict")0

### bytearray.decode(encoding="utf-8", errors="strict")

返回以指定格式进行编码的字符串，默认：utf-8

### bytes.endswith(suffix[, start[, end]])

### bytearray.endswith(suffix[, start[, end]])

如果二进制数据以指定后缀：suffix结束，则返回True

### bytes.find(sub[, start[, end]])

### bytearray.find(sub[, start[, end]])

查找sub在bytes中最低的索引位置，如果没有找到，则返回-1

### bytes.index(sub[, start[, end]])

### bytearray.index(sub[, start[, end]])

查找sub在bytes中最低的索引位置，如果没有找到，则返回一个异常

### bytes.join(iterable)

### bytearray.join(iterable)

以 iterable 为分隔符，分隔字节

### static bytes.maketrans(from, to)

### static bytearray.maketrans(from, to)

将字符串进行映射，from需要映射的迭代字符串，to映射后的迭代字符串，以下标进行映射。len(from)=len(to)
为translate()方法提供字符映射转换表

### bytes.partition(sep)

### bytearray.partition(sep)

在第一次出现sep时分割序列，并返回一个包含分隔符之前的部分、分隔符本身或其字节副本以及分隔符之后的部分的3元组。如果没有找到分隔符，则返回一个包含原始序列副本的3元组，后面跟着两个空字节或字节对象。
搜索的分隔符可以是任何字节，如对象。

### bytes.replace(old, new[, count])

### bytearray.replace(old, new[, count])

将旧序列old替换成新序列new，不超过count次。

### bytes.rfind(sub[, start[, end]])

### bytearray.rfind(sub[, start[, end]])

从右侧查找sub在bytes中最低的索引位置，如果没有找到，则返回-1

### bytes.rindex(sub[, start[, end]])

### bytearray.rindex(sub[, start[, end]])

从右侧查找sub在bytes中最低的索引位置，如果没有找到，则返回一个异常

### bytes.rpartition(sep)

### bytearray.rpartition(sep)

在bytes右侧sep第一次出现时分割序列，并返回一个包含分隔符之前的部分、分隔符本身或其字节副本以及分隔符之后的部分的3元组。如果没有找到分隔符，则返回一个包含原始序列副本的3元组，后面跟着两个空字节或字节对象。
搜索的分隔符可以是任何字节，如对象。

### bytes.startswith(prefix[, start[, end]])

### bytearray.startswith(prefix[, start[, end]])

如果数据以指定字符开头，则返回Tuer。

### bytes.translate(table, delete=b'')

### bytearray.translate(table, delete=b'')

传入maketrans()方法产生的映射对象table，将字符串中的映射对象进行替换，并且删除迭代对象delete中的字符。


