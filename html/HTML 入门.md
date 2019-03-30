#  HTML 入门

##  概念

* HTML 指的是超文本标记语言 (Hyper Text Markup Language) www万维网的描述性语言.

  ​	

##  基本结构

* ``` 
  <!DOCTYPE html>
  <html lang="en">
  <head>
  	<meta charset="UTF-8">
  	<title>Document</title>
  </head>
  <body>
  	
  </body>
  </html>
  ```

  

##  基本语法

1.  <常规语法>

   <标记 属性="属性值" 属性=“属性值”></标记>>

   标记也可叫标签或叫元素
   例如：<head></head>

2. 空标记

   <标记 属性=“属性值” />
   例如：<meta charset="utf-8">

   

##  常用标记

###  核心

​     *语义(核心)：从标签代表的意义上选择使用不同的标签，而不是根据标签的样式来决定*

###  标签

  <p></p>段落标签


 ```
<br>换行标签
<hr>换行分割线
<b>变粗的内容</b>只显示加粗
<strong>强调的内容</strong>突出的文本 强调优先级高
<i></i>	倾斜文本
<em></em> 强调文本  带有引用效果
<u></u>下划线
<del></del>删除线
<s></s>删除线
<sub></sub>居下，缩小字体
<sup></sup>居上，缩小字体
*无序列表
无序列表组成：
<ul>(unordered list)
<li></li>
<li></li>
．．．．．．
</ul>
*有序列表
有序列表组成：
<ol>(ordered list)
<li></li>
<li></li>
．．．．．．
</ol>
*自定义列表
<dl>(definition list)
<dt>名词</dt>
<dd>解释</dd>

<img src="目标文件路径及全称" alt="图片替换文本" title="图片标题" width="宽度" height="高度"/>

<a href="目标文件路径及全称/连接地址" title="提示文本">链接文本/图片</a>

<div ></div>
<span> </span>
 ```

##  常见现象

###  空白折叠

* 当我们在代码中写了很多空格，最终体现在网页上的只有一个空格

* 如果需要使用空格，应使用&nbsp；进行空格

  

###  自动换行

* 网页中，无论英文中文，浏览器自动会甄别当前词汇是否已经结束，如果没有结束，并且后面空间不足以容下一个词汇，那么浏览器会自动换行。
* 如果你在写英文的时候，没有使、用空格，那么浏览器就不会帮你把内容换行

##  全局属性

* tittle

  *Tips:除了基本的结构标签，例如<html><body>之类的可见标签都可以设置这个属性*

##  Form表单

*  作用:登录，注册，搜索

* 用法:通过form标签  input标签组合使用

* 常用属性:

  **密码：password
  提交：submit value(按钮内容)
  重置：reset
  单选框：type=“radio”
  多选框：type=“checkBox”
  默认选项：checked
  提示文本：placeholder**

