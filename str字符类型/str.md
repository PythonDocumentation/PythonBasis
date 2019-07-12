# 字符串类型

由固定不变的str类型表示，存放Unicode字符序列。

原始字符串：在字符串的前引号处加上r，用于解决转义处理。

## 字符串跨行表示：

```python
s = 'jiang'+ \
	'daoyi'

s = ('jiang'
	'dapyi')
```

## 多行字符串

```python
s = """
	jiang
	daoyi"""
```

## 字符串运算符

| +       | 字符串连接                                                   | a + b 输出结果： HelloPython                   |
| ------- | :----------------------------------------------------------- | ---------------------------------------------- |
| *       | 重复输出字符串                                               | a*2 输出结果：HelloHello                       |
| []      | 通过索引获取字符串中字符                                     | a[1] 输出结果 e                                |
| [ : ]   | 截取字符串中的一部分，取到截止点的前一个                     | a[1:4] 输出结果 ell                            |
| in      | 成员运算符 - 如果字符串中包含给定的字符返回 True             | H in a 输出结果 1                              |
| not in  | 成员运算符 - 如果字符串中不包含给定的字符返回 True           | M not in a 输出结果 1                          |
| r/R     | 原始字符串 - 原始字符串：所有的字符串都是直接按照字面的意思来使用，没有转义特殊或不能打印的字符。 原始字符串除在字符串的第一个引号前加上字母"r"（可以大小写）以外，与普通字符串有着几乎完全相同的语法。 | print r'\n' prints \n 和 print R'\n' prints \n |
| %       | 格式字符串                                                   | 请看下一节内容。                               |
| [ : : ] | 以跳固定步数的方式，截取字符串中的一部分                     | a[0:6:2] 输出结果：Hlo                         |

## 字符串内建函数

| 函数 | 用法 |
| ------------------------------------------------- | ------------------------------------------------------------ |
| str.   capitalize ()                              | 返回第一个字符转换为大写的字符串                             |
| str.   casefold ()                                | 返回全部转换为小写的   str ，能正确转换其他语言。   python 3.3 |
| str.   center (width, [,   fillchar])             | 返回一个指定的宽度   width 并且居中的字符串，fillchar   为填充的字符，默认为空格。   如果 width   < len(str)，则返回原始字符串。 |
| string.   count (str, beg= 0, end=len(string))    | 返回   str 在 string 里面出现的次数，如果   beg 或者 end 指定，则返回指定范围内   str 出现的次数 |
| str.   encode (encoding='UTF-8', errors='strict') | 以   encoding 指定的编码格式编码字符串，如果出错默认报一个ValueError   的异常，除非 errors 指定的是'ignore'或者'replace' |
| str.   endswith (suffix, beg=0, end=len(string))  | 检查字符串是否以   obj 结束，如果beg 或者   end 指定则检查指定的范围内是否以   obj 结束，如果是，返回 True,否则返回   False. |
| str.   expandtabs(tabsize=8)                      | 把字符串   str 中的 tab 符号转为空格，tab   符号默认的空格数是 8 |
| str.   find (string, beg=0 end=len(str))          | 检测   string 是否包含在字符串中，如果指定范围   beg 和 end ，则检查是否包含在指定范围内，如果包含返回开始的索引值，否则返回-1 |
| str.   format(*args, **kwargs)·                   | 字符串格式化函数，以序号或者变量名进行索引   python 3.7      |
| str.   format_map(mapping)                        | 字符串格式化函数，以字典的方式进行索引，索引直接被变量替代。   python 3.2 |
| index   (str, beg=0, end=len(string))             | 跟find   ()方法一样，只不过如果str不在字符串中会报一个异常.  |
| isalnum   ()                                      | 如果字符串至少有一个字符并且所有字符都是字母或数字则返 回   True,否则返回   False |
| isalpha   ()                                      | 如果字符串至少有一个字符并且所有字符都是字母则返回   True, 否则返回   False |
| str.   isascii ()                                 | 如果字符串为空或字符串中的所有字符为ASCII，返回true，否则为false。   ASCII字符的代码点在U+   0000u -U+007F的范围内。 |
| str.   isdecimal ()                               | 如果字符串都是十进制字符，且至少有一个字符则返回true，否则为false。 |
| isdigit   ()                                      | 如果字符串只包含数字则返回   True 否则返回   False.          |
| str.   isidentifier ()                            | 如果字符串是一个有效的标识符、语言定义、片段标识符和关键字，返回true。   使用keyword.iskeyword()来测试保留标识符，比如def和class。 |
| islower   ()                                      | 如果字符串中包含至少一个的字母，并且所有这些(区分大小写的)字母都是小写，则返回   True，否则返回 False |
| isnumeric   ()                                    | 如果字符串中至少有一字符并且只包含数字字符，则返回   True，否则返回 False |
| str.isprintable ()                             | 如果字符串的所有字符都是可打印的，或者为空，则返回True。否则返回False |
| isspace   ()                                      | 如果字符串是标题化的(见   title ())则返回   True，否则返回 False |
| str.   istitle ()                                 | 如果字符串是带标题的字符串，并且至少有一个字符，则返回true   |
| isupper   ()                                      | 如果字符串中包含至少一个字母，并且所有这些(区分大小写的)   字母都是大写，则返回 True，否则返回   False |
| str.   join (iterable)                            | iterable：可迭代的序列，str分隔符   返回序列以str为分隔符的字符串 |
| len(string)                                       | 返回字符串长度                                               |
| ljust   (width [, fillchar])                      | 返回一个原字符串左对齐,并使用   fillchar 填充至长度   width 的新字符串，fillchar   默认为空格 |
| lower   ()                                        | 转换字符串中所有大写字符为小写                               |
| lstrip   ()                                       | 截掉字符串左边的空格或指定字符                               |
| maketrans   ()                                    | 创建字符映射的转换表，对于接受两个参数的最简单的调用方式，第一个参数是字符串，表示需要转换的字符，第二个参数也是字符串表示转换的目标 |
| max(str)                                          | 返回字符串   str 中最大的字母                                |
| min(str)                                          | 返回字符串   str 中最小的字母                                |
| partition(sep)                                    | 在sep第一次出现时拆分字符串，并返回一个包含分隔符前部分、分隔符本身和分隔符后部分的3元组。如果没有找到分隔符，返回一个包含字符串本身的3元组，后面跟着两个空字符串。 |
| replace   (old, new [, max])                      | 将字符串中的   str1 替换成   str2,如果   max 指定，则替换不超过 max 次 |
| rfind   (str, beg=0, end=len(string))             | 类似于   find ()函数，不过是从右边开始查找                   |
| rindex   (str, beg=0, end=len(string))            | 类似于   index ()，不过是从右边开始                          |
| rjust   (width, [, fillchar])                     | 返回一个原字符串右对齐,并使用fillchar(默认空格）填充至长度   width 的新字符串 |
| rpartition(sep)                                   | 从右边开始查找，在sep第一次出现时拆分字符串，并返回一个包含分隔符前部分、分隔符本身和分隔符后部分的3元组。如果没有找到分隔符，返回一个包含字符串本身的3元组，后面跟着两个空字符串。 |
| rstrip   ()                                       | 删除字符串字符串末尾的空字符，或删除指定字符。               |
| split   (str="", num=string. count(str))          | num=string.count(str)) 以   str 为分隔符截取字符串,分割后   str 被删除，如果 num 有指定值，则仅截取   num 个子字符串。若 str 为空值则以不可见字符为切割符。将字符串切割成列表 |
| splitlines   ([keepends])                         | 按照行('\r',   '\r\n', \n')分隔，返回一个包含各行作为元素的列表，如果参数   keepends 为   False，不包含换行符，如果为   True，则保留换行符。 |
| startswith   (str, beg=0, end=len(string))        | 检查字符串是否是以   obj 开头，是则返回 True，否则返回   False。如果beg   和 end 指定值，则在指定范围内检查 |
| strip([chars])                                    | 在字符串上执行   lstrip ()和   rstrip ()，是将字符串的左侧和右侧字符切割，而不是居中 |
| swapcase   ()                                     | 将字符串中大写转换为小写，小写转换为大写                     |
| title   ()                                        | 返回"标题化"的字符串,就是说所有单词都是以大写开始，其余字母均为小写(见   istitle  ()) |
| translate   (table, deletechars="")               | 根据   str 给出的表(包含   256 个字符)转换   string 的字符,   要过滤掉的字符放到 deletechars 参数中 |
| upper   ()                                        | 转换字符串中的小写字母为大写                                 |
| zfill   (width)                                   | 返回长度为   width 的字符串，原字符串右对齐，前面填充0       |



3. 