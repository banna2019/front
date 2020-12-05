### HTML

##### 0.创建HTML文件

###### 新建项目

![image-20201205193501398](/Users/banna/Library/Application Support/typora-user-images/image-20201205193501398.png)

![image-20201205193555583](/Users/banna/Library/Application Support/typora-user-images/image-20201205193555583.png)



新建html文件

![image-20201205193650343](/Users/banna/Library/Application Support/typora-user-images/image-20201205193650343.png)



##### 1.HTML文档结构

```html
<!DOCTYPE html>
<html>
  <head>
    <!--网页的头部-->
  </head>
  <body>
    <!--网页内容-->
  </body>
</html>
```



###### 运行代码

![image-20201205193905390](/Users/banna/Library/Application Support/typora-user-images/image-20201205193905390.png)

![image-20201205195127164](/Users/banna/Library/Application Support/typora-user-images/image-20201205195127164.png)





##### 2.HTML文档注释

```html
<!-- -->	用于注释代码
```



##### 3.HTML元素关系

```html
父子关系
<html>	<head>
<html>	<body>

<head> <title>

子孙关系
<html>	<title>  
```



##### 4.HTML常用标签

###### 1.基础标签

​	html 最外层的元素

​	head 网页的头部

​		meta charset=	声明网页的语言

​	title	网页的标题

​	body	网页内容



###### 2.文本格式化(内容标签)

​	i/em	斜体

```html
<i>武汉,加油！</i>
<em>武汉,加油！</em>
```



​	strong	加粗

```html
<em><strong>武汉,加油！</strong></em>	//可以嵌套使用
```



​	q 	引用(短引用)

```html
<q>江湖险恶,保命要紧</q>
```



​	blockquote	长引用

```html
		<blockquote>
			江湖险恶,保命要紧
		</blockquote>
```



​	code	元素定义编程代码示例

```html
<code> var a = 1 </code>
```



![image-20201205202338384](/Users/banna/Library/Application Support/typora-user-images/image-20201205202338384.png)





###### 3.标题段落

​	h1-h6	表示标题 数字越大 字体越小

​	p	段落标签

​	hr	水平分割线

​	br 换行

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>使用标题和段落</title>
	</head>
	<body>
			<!-- 标题 -->
		<h1>武汉加油!</h1>
		<h2>武汉加油!</h2>
		<h3>武汉加油!</h3>
		
		<h4>武汉加油!</h4>
		<h5>武汉加油!</h5> 
		<h6>武汉加油!</h6>
		
			<!-- 段落标签 -->
		<p>武汉加油! 武汉加油! 武汉加油! 武汉加油! 武汉加油! 武汉加油! 武汉加油!</p>
		
		<hr >	<!--水平分割线-->
		<p>武汉加油! 武汉加油! 武汉加油! 武汉加油! 武汉加油! 武汉加油! 武汉加油!</p>
		
		武汉加油! 武汉加油! 
		<br>武汉加油! 武汉加油! 	<!--换行-->
	</body>
</html>

```

![image-20201205205124698](/Users/banna/Library/Application Support/typora-user-images/image-20201205205124698.png)



###### 4.块元素

​	div 盒子(容器)	//在多行显示

​	span	功能和div类似,span可以用来装一小段文件和div的区别就是 在一行内像是

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>03</title>
	</head>
	<body>
		<i style="background-color: blue;">武汉加油！武汉加油！武汉加油！武汉加油！</i>
		<div style="background-color: aqua;">
			武汉加油！武汉加油！武汉加油！武汉加油！
		</div>
		<div style="background-color: aqua;">
			武汉加油！武汉加油！武汉加油！武汉加油！
		</div>
		
		<span style="background-color: blue;">
			武汉加油！武汉加油！武汉加油！武汉加油！
		</span>
		<span style="background-color: blue;">
			武汉加油！武汉加油！武汉加油！武汉加油！
		</span>
	</body>
</html>
```

![image-20201205210145176](/Users/banna/Library/Application Support/typora-user-images/image-20201205210145176.png)





###### 5.图片

​	img

​		img标签必须加上src属性 才能把图像展示出来

​		alt属性: 当图片没有办法显示的时候用来提示用户的文字title属性;当鼠标移动到图片的时候,用来提示用户的文字

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>使用图片</title>
	</head>
	<body>
		<img src="images/01.png" alt="风景图" title="测试图片" >
	</body>
</html>
```

![image-20201205211620284](/Users/banna/Library/Application Support/typora-user-images/image-20201205211620284.png)



###### 6.链接

​	a标签: 超链接的地址

​		href属性: 超链接的地址

​		target属性: _blank表示新建一个浏览器标签页来显示超链接的内容,不会覆盖原来的网页

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>链接</title>
	</head>
	<body>
		<a href="http://www.baidu.com" target="_blank">百度一下</a>	<!--重新生成一个页面,进行跳转-->
		<a href="http://www.baidu.com" target="_parent">百度一下</a>	<!--直接跳转到指定页面,会覆盖当前页面-->
		<a href="http://www.baidu.com" target="_search">百度一下</a>	<!--重新生成一个页面,进行跳转-->
		<a href="http://www.baidu.com" target="_self">百度一下</a>	<!--直接跳转到指定页面,会覆盖当前页面-->
		<a href="http://www.baidu.com" target="_top">百度一下</a>		<!--直接跳转到指定页面,会覆盖当前页面-->
	</body>
</html>
```

![image-20201205212619645](/Users/banna/Library/Application Support/typora-user-images/image-20201205212619645.png)



###### 7.列表

​	ol	有序列表

​	ul	无序列表

​	li	列表项

​		type定义类型

​			disc	实体圆点

​			circle	空心圆

​			square	实体方形

​			a 小写字母(有序)

​			A 大写字母(有序)

​			默认数字(有序)

```html
<!--无序列表-->
<h4>职位信息: </h4>
<ul type="disc">
  <li>开发工程师</li>
  <li>运维工程师</li>
  <li>测试工程师</li>
	<li>产品经理</li>
</ul>

<!--有序列表-->
<h4>数字列表</h4>
<ol>
  <li>开发工程师</li>
  <li>运维工程师</li>
  <li>测试工程师</li>
  <li>产品经理</li>
</ol>
```



​		





