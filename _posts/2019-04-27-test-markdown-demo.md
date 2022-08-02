---
layout: post
title: 测试 markDown 语法
subtitle: markDown 基本语法测试
tags: [test]
comments: true
---

写过博客或者github上面的文档的，应该知道Markdown语法的重要性，不知道的朋友们也别着急，一篇博客轻松搞定Markdown语法。话说这个语法超级简单，一看就会，不信你点进来看看。

##1.基本语法

###1.1 标题

    #  H1
    ##  H2
    ###  H3
    ####  H4
    #####  H5
    ######  H6
 
**效果：**

#  H1
##  H2
###  H3
####  H4
#####  H5
######  H6

另外，H1和H2还能用以下方式显示：

    这是一级标题
    ===
**效果：**

这是一级标题
===

  
    这是二级标题
    ---
    
**效果：**

这是二级标题
---
    
###1.2 字体设置粗体、斜体、删除线

    **粗体abc** ，__粗体abc__  
    *斜体abc* ， _斜体abc_  
    ~~删除线abc~~

**效果：**

**粗体abc** ，__粗体abc__  
*斜体abc* ， _斜体abc_  
~~删除线abc~~

###1.2 列表

Unsordered 无序列表：

    * 无序列表
    * 子项
    * 子项
     
    + 无序列表
    + 子项
    + 子项
     
    - 无序列表
    - 子项
    - 子项

**效果：**

* 无序列表
* 子项
* 子项
 
+ 无序列表
+ 子项
+ 子项
 
- 无序列表
- 子项
- 子项

有序列表：

    1. 第一行
    2. 第二行
    3. 第三行

**效果：**

1. 第一行
2. 第二行
3. 第三行

**组合：**

    * 产品介绍（子项无项目符号）
        此时子项，要以一个制表符或者4个空格缩进
     
    * 产品特点
        1. 特点1
        - 特点2
        - 特点3
    * 产品功能
        1. 功能1
        - 功能2
        - 功能3
**效果：**

* 产品介绍（子项无项目符号）  
    此时子项，要以一个制表符或者4个空格缩进
 
* 产品特点
    1. 特点1
    - 特点2
    - 特点3
* 产品功能
    1. 功能1
    - 功能2
    - 功能3
    
###1.3 链接

Inline-style 内嵌方式：

    [link text](https://www.baidu.com")
    
 [link text](https://www.baidu.com "title text")
 
Reference-style 引用方式：

    [link text][id]
    
    [id]: https://www.baidu.com "title text"
    
[link text][id]

[id]: https://www.baidu.com "title text"
 
 
Relative reference to a repository file 引用存储文件：

    [link text](../path/file/readme.text "title text")
 
还能这样使用：

    [link text][]
    
    [link text]: https://www.baidu.com
    
[link text][]

[link text]: https://www.baidu.com
 
Email 邮件：

    Email <example@example.com>

Email<example@example.com>

###1.4 Images 图片

**Inline-style 内嵌方式：**

    ![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "title text")
 
 ![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "title text")

**Reference-style 引用方式：**

    ![alt text][logo]
    
    [logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "title text"

![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "title text"

###1.5 Code and Syntax Highlighting 代码和语法高亮

标记一小段行内代码：

本文是一篇介绍`Markdown`的语法的文章
 
如果高亮的内容包含`号，可以这样写：

    `` `包裹起来` ``
 
语法高亮：

    ```html
        <div>Syntax Highlighting</div>
    ```
    ```css
        body{font-size:12px}
    ```
     
    ```javascript
        var s = "JavaScript syntax highlighting";
        alert(s);
    ```
    ```php
        <?php
          echo "hello, world!";
        ?>
    ```
    ```python
        s = "Python syntax highlighting"
        print s
    ```
```html
    <div>Syntax Highlighting</div>
```
```css
    body{font-size:12px}
```
 
```javascript
    var s = "JavaScript syntax highlighting";
    alert(s);
```
```php
    <?php
      echo "hello, world!";
    ?>
```
```python
    s = "Python syntax highlighting"
    print s
```

###1.6 Block Code 代码分组(代码区块)：

在该行开头缩进4个空格或一个制表符(tab)

###1.7 <strong>Blockquotes 引用：</strong>

    > Email-style angle brackets
    > are used for blockquotes.
    > > And, they can be nested.
    > #### Headers in blockquotes
    > * You can quote a list.
    > * Etc.
    
> Email-style angle brackets
> are used for blockquotes.
> > And, they can be nested.
> #### Headers in blockquotes
> * You can quote a list.
> * Etc.


###1.8 Hard Line Breaks 换行：

在一行的结尾处加上2个或2个以上的空格，也可以使用`</br>`标签

    第一行文字<br>第二行文字
    
第一行文字<br>第二行文字  

###1.9 Horizontal Rules 水平分割线：

    ***
    ---
    * * *
    - - -
    
***
---
* * *
- - -

###1.11 Escape character 转义符(反斜杠)：
Markdown 可以利用反斜杠来插入一些在语法中有其它意义的符号，例如：如果你想要用星号加在文字旁边的方式来做出强调效果，你可以在星号的前面加上反斜杠：

    \*literal asterisks\*
   
\*literal asterisks\*
    
Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号：

\反斜杠  `反引号  *星号  _下划线  {}花括号  []方括号  ()括弧  #井字号  +加号  -减号  .英文句 !感叹号


###1.10 资源
Markdown官网：http://daringfireball.net/projects/markdown/
参考资料：http://markdown.tw/

Markdown在线编辑器：
Dillinger：http://dillinger.io/
Markdown Here：http://markdown-here.com/livedemo.html
