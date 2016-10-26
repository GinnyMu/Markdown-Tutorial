<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>

#<span id = "jump">入门教程</span>

## 标题格式 - 增加#的个数来减小标题字号 ##

代码格式:

    #一级标题
    ##二级标题
    ###三级标题
    ####四级标题
    #####五级标题
    ######六级标题
 
    
显示效果:
> #一级标题
> ##二级标题
> ###三级标题
> ####四级标题
> #####五级标题
> ######六级标题


##列表:
###无序列表 : 在文本前加入- 即可
代码格式:
    
    - 第一行
    - 第二行
    - 第三行

显示效果:

- 第一行
- 第二行
- 第三行

###有序列表: 在文字前加入1. 2. 3. ,以下为例:
代码格式:

    1. 文本1
    2. 文本2
    3. 文本3


显示效果:

1. 文本1
2. 文本2
3. 文本3


###缩进效果:加三个空格跳转下一级
代码格式:

```
- 第一层
   - 第二层
      - 第三层
```
显示效果:
- 第一层
   - 第二层
      - 第三层

 

## 文字引用与文字格式:  ##
### 文字引用: 在文字前加入>, 并在空格后输入引用的文字:

#### 引用:
    
    > 这是一段引用

显示:

> 这是一段引用

####  多级引用:
代码:
    
    > 这是一级引用
    > >这是二级引用
    > > >这是三级引用

    > > 这是二级引用
    > 这并不是一级引用
    

NOTE: 如果>和>>嵌套使用的话，从>>退到>时，必须之间要加一个空格或者>作为过渡，否则默认为下一行和上一行是同一级别的引用。如示例所示。

显示:

> 这是一级引用
> >这是二级引用
> > >这是三级引用

> > 这是二级引用
> 这并不是一级引用

### 文字格式: ###
#### 斜体: 

*斜体*  _斜体_

代码:

    *斜体*或者_斜体_

#### 黑体: 

**黑体** __黑体__

代码:

    **黑体**或者__黑体__

#### 加入空格: 

因为若加入两个以上空格之后换行, 所以采用shift+space开启全角空格来达到空格的目的.
代码：
```
　　　　　　
```

#### 删除线:

~~这是一条删除线~~

代码:
```
~~这是一条删除线~~
```

#### 分割线:


使用`---`或者`***`或者` * * *` 表示水平分割线。

Note:
只要*或者-大于等于三个就可组成一条平行线。
使用`---`作为水平分割线时，要在它的前后都空一行，防止`---`被当成标题标记的表示方式。

#### 标签

```
标签: 数学 英语 
Tags: 数学 英语
```
#### 注脚:

```
这是一个注脚测试[^footer1]。
[^footer1]: 这是一个测试，用来阐释注脚。
```
这是一个注脚测试[^footer1]。
[^footer1]: 这是一个测试，用来阐释注脚。
## 代码引用: ##
###单行代码引用:  在代码左右两侧加 ` ###

    `code`

### 多行代码引用: 在代码首行和末行都加入 ```, 例如:  

    ``` 
    abcd
    efgh
    ijkl
    ``` 

##链接及图片:
###链接: 格式为`[显示文本](图片链接)`: 
` [baidu](www.baidu.com)` -- [baidu](www.baidu.com)
### 图片: 格式为:
`![](https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcSCWAXj6NGZdqOG-ds7bCAHXNI6x06gLeAhp3P5h4LEPEAdbnFc)`:
![](https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcSCWAXj6NGZdqOG-ds7bCAHXNI6x06gLeAhp3P5h4LEPEAdbnFc)
###另一种显示图片的方法


    ![][1]
    [1]:https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcSCWAXj6NGZdqOG-ds7bCAHXNI6x06gLeAhp3P5h4LEPEAdbnFc

![][1]
[1]:https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcSCWAXj6NGZdqOG-ds7bCAHXNI6x06gLeAhp3P5h4LEPEAdbnFc
##表格: 
* ------:为右对齐。 
* :------为左对齐。 
* :------:为居中对齐。 
* -------为使用默认居中对齐。

相关代码:

    | Tables | Are | Cool |
    | ------------- |:-------------:| -----:|
    | col 3 is | right-aligned | $1600 |
    | col 2 is | centered | $12 |
    | zebra stripes | are neat | $1 |

显示效果:

| Tables | Are | Cool |
| ------------- |:-------------:| :-----:|
| col 3 is | right-aligned | $1600 |
| col 2 is | centered | $12 |
| zebra stripes | are neat | $1 |

相关代码:
    
    
    dog | bird | cat
    ----|------|----
    foo | foo | foo
    bar | bar | bar
    
显示效果:

dog | bird | cat
----|------|----
foo | foo | foo
bar | bar | bar
baz | baz | baz

##数学公式插入：
Markdown的数学公式支持LaTex的数学公式书写格式, 所以一般可以在LaTex里面写完以后再通过图片转到Markdown里面, 也可以通过[在线数学公式](http://www.forkosh.com/mathtextutorial.html)来生成LaTex公式.

###方法1：使用Google Chart的服务器

    
    <img src="http://chart.googleapis.com/chart?cht=tx&chl= 在此插入Latex公式">

例如：
<img src="http://chart.googleapis.com/chart?cht=tx&chl=\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}">
    
    <img src="http://chart.googleapis.com/chart?cht=tx&chl=\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}">

### 方法2: 使用forkosh服务器
    
    <img src="http://www.forkosh.com/mathtex.cgi? 在此处插入Latex公式">

例如:
<img src="http://www.forkosh.com/mathtex.cgi? \Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}">

    <img src="http://www.forkosh.com/mathtex.cgi? \Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}">
    
###方法3: 使用MathJax引擎(因为Github中不支持markdwon对插入js脚本的解析，所以直接在Github上不好用，但使用pandoc转html和使用Markdown Preview Plus插件预览时都能用)


$$x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$$
\\(x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}\\)
##页面内跳转：
###页面内跳转
[跳转到头](#jump)


```
[跳转到头](#jump)
#<span id = "jump">入门教程</span>
```

###目录:在笔记开头写上"[Toc]"
