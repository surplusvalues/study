# markdown

## 标题

**使用 = 和 - 标记一级和二级标题**

= 和 - 标记语法格式如下：

```
我展示的是一级标题
=================

我展示的是二级标题
-----------------
```

显示效果如下图：![img](Markdown .assets/01986C87-7E19-4497-878E-AE996AFC088E.jpg)

**使用 # 号标记**

使用 **#** 号可表示 1-6 级标题，一级标题对应一个 **#** 号，二级标题对应两个 **#** 号，以此类推。

```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

显示效果如下图：![img](Markdown .assets/md2.gif)

## 段落

Markdown 段落没有特殊的格式，直接编写文字就好，**段落的换行是使用两个以上空格加上回车**![img](Markdown .assets/36A89BDA-A062-4D66-A41B-0EBEE7891AB9.jpg)

当然也可以在段落后面使用一个空行来表示重新开始一个段落。![img](Markdown .assets/3F254936-778E-417A-BEF2-467116A55D00.jpg)

### 字体

Markdown 可以使用以下几种字体：

```
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___
```

显示效果如下所示：

![img](Markdown .assets/md3.gif)

### 分隔线

你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：

```
***

* * *

*****

- - -

----------
```

显示效果如下所示：![img](Markdown .assets/3F46EAA9-DADE-48FD-99AA-DF7BEBFAA4FA.jpg)

### 删除线

如果段落上的文字要添加删除线，只需要在文字的两端加上两个波浪线 **~~** 即可，实例如下：

```
RUNOOB.COM
GOOGLE.COM
~~BAIDU.COM~~
```

显示效果如下所示：![img](Markdown .assets/B5270A31-15D0-410B-AE1D-B9655B8F331C.jpg)

### 下划线

下划线可以通过 HTML 的 **<u>** 标签来实现：

```
<u>带下划线文本</u>
```

显示效果如下所示：

![img](Markdown .assets/05A27273-B66D-43DE-A3DB-0D32FF024093.jpg)

### 脚注

脚注是对文本的补充说明。

Markdown 脚注的格式如下:

```
[^要注明的文本]
```

以下实例演示了脚注的用法：

```
创建脚注格式类似这样 [^RUNOOB]。

[^RUNOOB]: 菜鸟教程 -- 学的不仅是技术，更是梦想！！！
```

演示效果如下：![img](Markdown .assets/md5.gif)

## 列表

Markdown 支持有序列表和无序列表。

无序列表使用星号(*****)、加号(**+**)或是减号(**-**)作为列表标记，这些标记后面要添加一个空格，然后再填写内容：

```
* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项


- 第一项
- 第二项
- 第三项
```

显示结果如下：![img](Markdown .assets/89446A8E-6D83-4666-AACC-980145D5F070.jpg)

有序列表使用数字并加上 **.** 号来表示，如：

```
1. 第一项
2. 第二项
3. 第三项
```

显示结果如下：![img](Markdown .assets/560384BB-2B00-41D5-ACF2-18972F7F2775.jpg)

**列表嵌套**

列表嵌套只需在子列表中的选项前面添加两个或四个空格即可：

```
1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素
```

显示结果如下：![img](Markdown .assets/8ED795DA-F124-4E70-BA71-57CD9CF958A4.jpg)

## 区块

Markdown 区块引用是在段落开头使用 **>** 符号 ，然后后面紧跟一个**空格**符号：

```
> 区块引用
> 菜鸟教程
> 学的不仅是技术更是梦想
```

显示结果如下：![img](Markdown .assets/DFE1124E-BC38-4C12-B7AC-053E560D4C9C.jpg)

另外区块是可以嵌套的，一个 **>** 符号是最外层，两个 **>** 符号是第一层嵌套，以此类推：

```
> 最外层
> > 第一层嵌套
> > > 第二层嵌套
```

显示结果如下：![img](Markdown .assets/AA0A4A6A-33A7-48C7-971F-73FFC8FE85B0.jpg)

**区块中使用列表**

区块中使用列表实例如下：

```
> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> + 第二项
> + 第三项
```

显示结果如下：![img](Markdown .assets/E3BF6399-6483-4C7A-8502-AE75E8D66C96.jpg)

**列表中使用区块**

如果要在列表项目内放进区块，那么就需要在 **>** 前添加四个空格的缩进。

列表中使用区块实例如下：

```
* 第一项
    > 菜鸟教程
    > 学的不仅是技术更是梦想
* 第二项
```

显示结果如下：![img](Markdown .assets/1B894FB4-53AC-4E2D-BA30-F4AE4DFA8B97.jpg)

## 代码

**如果是段落上的一个函数或片段的代码可以用反引号把它包起来（`），例如：**

```
`printf()` 函数
```

显示结果如下：![img](Markdown .assets/C928FDA3-E0A7-4AFF-AB2A-B3AF44F93DF9.jpg)

**代码区块**

代码区块使用 **4 个空格**或者一个**制表符（Tab 键）**。

实例如下：

![img](Markdown .assets/55EDFE05-5F27-458E-AFE0-7B96685C9603.jpg)

显示结果如下：![img](Markdown .assets/6DC89E5C-B41A-4938-97D8-D7D06B879F91.jpg)

**你也可以用 ``` 包裹一段代码，并指定一种语言（也可以不指定）：**

````
```javascript
$(document).ready(function () {
    alert('RUNOOB');
});
```
````

显示结果如下：![img](Markdown .assets/88F52386-2F98-4D7E-8935-E43BECA6D868.jpg)

## 链接

链接使用方法如下：

```
[链接名称](链接地址)

或者

<链接地址>
```

例如：

```
这是一个链接 [菜鸟教程](https://www.runoob.com)
```

显示结果如下：![img](Markdown .assets/49E6CB42-F780-4DA6-8290-DC757B51FB9A.jpg)

直接使用链接地址：

```
<https://www.runoob.com>
```

显示结果如下：![img](Markdown .assets/9BFF60A1-DD71-4B63-987B-4665B31C7787.jpg)

**高级链接**

我们可以通过变量来设置一个链接，变量赋值在文档末尾进行：

```
这个链接用 1 作为网址变量 [Google][1]
这个链接用 runoob 作为网址变量 [Runoob][runoob]
然后在文档的结尾为变量赋值（网址）

  [1]: http://www.google.com/
  [runoob]: http://www.runoob.com/
```

显示结果如下：![img](Markdown .assets/EC3ED5D2-4F0D-492A-81B3-D485623D1A9E.jpg)

## 图片

Markdown 图片语法格式如下：

```
![alt 属性文本](图片地址)

![alt 属性文本](图片地址 "可选标题")
```

- 开头一个感叹号 !
- 接着一个方括号，里面放上图片的替代文字
- 接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 'title' 属性的文字。

使用实例：

```
![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")
```

显示结果如下：![img](Markdown .assets/A042DF30-C232-46F3-8436-7D6C35351BBD.jpg)

当然，你也可以像网址那样对图片网址使用变量:

```
这个链接用 1 作为网址变量 [RUNOOB][1].
然后在文档的结尾为变量赋值（网址）

[1]: http://static.runoob.com/images/runoob-logo.png
```

显示结果如下：![img](Markdown .assets/75AA6EBF-CC57-44A6-A585-5EE3DD94E42A.jpg)

Markdown 还没有办法指定图片的高度与宽度，如果你需要的话，你可以使用普通的 <img> 标签。

```
<img decoding="async" src="http://static.runoob.com/images/runoob-logo.png" width="50%">
```

显示结果如下：![img](Markdown .assets/55F2A67D-F4BD-4960-AC55-DC690A415878.jpg)

## 表格

Markdown 制作表格使用 **|** 来分隔不同的单元格，使用 **-** 来分隔表头和其他行。

语法格式如下：

```
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |
```

以上代码显示结果如下：![img](Markdown .assets/23EACC50-38E0-4284-B99A-6BC22E284BAC.jpg)

对齐方式

**我们可以设置表格的对齐方式：**

- **-:** 设置内容和标题栏居右对齐。
- **:-** 设置内容和标题栏居左对齐。
- **:-:** 设置内容和标题栏居中对齐。

实例如下：

```
| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |
```

以上代码显示结果如下：![img](Markdown .assets/87DE9D5C-44FB-4693-8735-194D3779EC3E.jpg)





## 高级技巧

见        [菜鸟教程](https://www.runoob.com/markdown/md-advance.html)

