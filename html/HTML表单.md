#  HTML5

##  相对路径与绝对路径

1.  相对路径
   * 从发问者角度讲问题

2. 绝对路径
   * 从根源位置开始阐述

Tips:一般情况下推荐使用相对路径,即可以省服务器读取速度,也可以减少不必要的麻烦.

##  图片

```
<img src="图片路径" alt="加载失败所提示的信息"></img>
```

* src: 图片路径,也就是图片所存储的位置.建议使用相对路径去阐述.
* alt:图片加载失败时,所显示的文本信息,主要用来提升网页评分,并增强用户体验度.
* 图片可以设置宽高
  * width 宽
  * height 高

##  按钮

###  submit

* 形成的按钮只是用来提交数据

###  button

* 普通按钮,主要配合JavaScript组合使用

##  全局属性ID

* 属性值不可以重复

##  表单

### 作用

* 用来收集用户信息

### 组成

* 表单框(表单域form)
* 提示信息
* 表单控件/表单元素

### 属性

* 表单框

  * ```
    <form name="表单名称（英文字母开头的）" method（提交方式）="post/get" action="表单提交的地址"></form>
    ```

    

* input标签 type属性值

  1. text :文本框

  2. password :密码框

  3. submit :提交按钮

  4. reset :重置按钮

  5. radio :单选框

  6. checkbox :复选框

  7. select 与 option  :下拉菜单(name值必须相等)

     ```
     <select name="">
     <option name="" value="表单被提交时被发送到服务器的值">菜单内容</option>
     </select>
     ```

  8. textarea :多行文本域

     ```
     <textarea name="textareal" cols="字符宽度" rows="行数">
     </textarea>
     
     ```

  9. button :提交按钮

  10. checked :为默认选项

      ```
      <input type="radio" checked="checked" />
      ```

  11. disabled :禁用状态

  12. enabled :可用状态

  13.  placeholder :提示文本

###  value 的不同语境

* value 属于input 元素设定值,对于不同输入类型,属性用法也不相同

  >
  >
  >type="button", "reset", "submit" - 定义按钮上的显示的文本
  >type="text", "password" - 定义输入字段的初始值
  >type="checkbox", "radio" - 定义与输入相关联的值

###  get与post的区别

* get,post都是从Form表单中获取数据的方式

  ####  区别:

  1.   get是从服务器上获取数据，post是向服务器传送数据。

  2. get是把参数数据队列加到提交表单的ACTION属性所指的URL中，值和表单内各个字段一一对应，在URL中可以看到。post是通过HTTP post机制，将表单内各个字段与其内容放置在HTML HEADER内一起传送到ACTION属性所指的URL地址。用户看不到这个过程。

  3. 对于get方式，服务器端用Request.QueryString获取变量的值，对于post方式，服务器端用Request.Form获取提交的数据。

  4. get传送的数据量较小，不能大于2KB。post传送的数据量较大，一般被默认为不受限制。

  5. get安全性非常低，post安全性较高。但是执行效率却比Post方法好.

     

  

  ####  总结

  1.  get方式的安全性较Post方式要差些，包含机密信息的话，建议用Post数据提交方式；
  2. 在做数据查询时，建议用Get方式；而在做数据添加、修改或删除时，建议用Post方式；

##  div与span 的用法

###  div

* 没有具体含义， 除了独占一行之外没有任何其它的默认属性，是页面布局中常用的标签；

  

###  span

* 可以是某一小段文本，或是某一个字。 它除了不换行外，没有任何其它的默认属性； 