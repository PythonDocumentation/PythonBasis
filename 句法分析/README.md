# 句法分析

Python 程序由一个 *解析器* 读取。输入到解析器的是一个由 *词法分析器* 所生成的 *形符* 流，本章将描述词法分析器是如何将一个文件拆分为一个个形符的。

Python 会将读取的程序文本转为 Unicode 码点；源文件的文本编码可由编码声明指定，默认为 UTF-8，详情见 [**PEP 3120**](https://www.python.org/dev/peps/pep-3120)。如果源文件无法被解码，将会引发 [`SyntaxError`](https://docs.python.org/zh-cn/3/library/exceptions.html#SyntaxError)。

