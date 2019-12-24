# 算法部分day1作业

## 练习1

### a. 题目

请设计一个函数,该函数接收一个字符串.该字符串表示一段HTML代码.该函数返回值为布尔值.该布尔值表示HTML代码中的标签是否匹配.如匹配返回True,否则返回False.

- 1. 待检测的HTML代码中,标签均为成对出现.即:无单标签.
- 2. HTML代码的文本内容中(如例子中的Title和Hello World)无与标签内容相同的字面量

例:

```python
html_content = """
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Title</title>
</head>
<body>
    <h1>Hello World</h1>
</body>
</html>
"""

html_content2 = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>
    <h1>Hello<h2> World</h1></h2>
</body>
</html>
"""


def check_html_match(html_content):
    """
    本函数用于检测一段HTML代码中 标签嵌套是否正确 标签是否匹配
    :param html_content: string
    :return: bool
    """
```

则有:

- 对于`html_content`,则函数`check_html_match()`返回值为True;
- 对于`html_content2`,则函数`check_html_match()`返回值为False;

### b. 要求

- 1. 请将完成后的代码提交至**个人github**,并在微信群内告知个人github地址.
- 2. 代码完成后,请从代码的**简洁性**和**可读性**两个方面进行改进,每次改进后请将改进结果提交至github.改进工作基于原文件进行即可.
- 3. 作业提交截止日期:2020年1月3日.
- 4. 在自身实现功能的前提下,尽可能对对方的代码作出coding review.

