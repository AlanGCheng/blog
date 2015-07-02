HTML学习笔记
1.标题
<h1>This is a heading</h1>
<h1>~<h6>逐渐变小

2.段落
<p>This is a paragraph.</p>

3.链接
<a href="http://www.w3school.com.cn">This is a link</a>

4.图像
<img src="w3school.jpg" width="104" height="142" />

5.换行
<br>

6.水平线
<p>This is a paragraph</p>
<hr />
<p>This is a paragraph</p>
<hr />
<p>This is a paragraph</p>
可以用于分离文章中的小节

7.注释
<!-- This is a comment -->

8.查看源代码
如果您想找到其中的奥秘，只需要单击右键，然后选择“查看源文件”（IE）或“查看页面源代码”（Firefox），其他浏览器的做法也是类似的。这么做会打开一个包含页面 HTML 代码的窗口。

要揭示一个网站的技术秘密，其实很简单。单击浏览器的“查看”菜单，选择“查看源文件”即可。随后你会看到一个弹出的窗口，窗口内就是实际的 HTML 代码。

9.换行
在不产生一个新段落的情况下进行换行（新行），请使用 <br /> 标签：
<p>This is<br />a para<br />graph with line breaks</p>

10.预留格式标签——适合显示代码
<pre>
for i = 1 to 10
     print i
next i
</pre>

11.代码显示
<code>Computer code</code>
<br />
<kbd>Keyboard input</kbd>
<br />
<tt>Teletype text</tt>
<br />
<samp>Sample text</samp>
<br />
<var>Computer variable</var>
<br />

<code> 定义计算机代码。 
<kbd> 定义键盘码。 
<samp> 定义计算机代码样本。 
<tt> 定义打字机代码。 
<var> 定义变量。 
<pre> 定义预格式文本。 


12.地址显示
<address>
Written by <a href="mailto:webmaster@example.com">Donald Duck</a>.<br> 
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>

13.隐藏信息，缩略信息
<abbr title="etcetera">etc.</abbr>
<br />
<acronym title="World Wide Web">WWW</acronym>

在某些浏览器中，当您把鼠标移至缩略词语上时，title 可用于展示表达的完整版本

14.改变文字输出方向

如果您的浏览器支持 bi-directional override (bdo)，下一行会从右向左输出 (rtl)；

<bdo dir="rtl">
Here is some Hebrew text
</bdo>

15.引用格式
这是长的引用：
<blockquote>
这是长的引用。这是长的引用。这是长的引用。这是长的引用。这是长的引用。这是长的引用。这是长的引用。这是长的引用。这是长的引用。这是长的引用。这是长的引用。
</blockquote>

这是短的引用：
<q>
这是短的引用。
</q>

<abbr> 定义缩写。 
<acronym> 定义首字母缩写。 
<address> 定义地址。 
<bdo> 定义文字方向。 
<blockquote> 定义长的引用。 
<q> 定义短的引用语。 
<cite> 定义引用、引证。 
<dfn> 定义一个定义项目。 


16.删除和下划线标示
<p>一打有 <del>二十</del> <ins>十二</ins> 件。</p>

17.常用文本格式化标签

<b> 定义粗体文本。 
<big> 定义大号字。 
<em> 定义着重文字。 
<i> 定义斜体字。 
<small> 定义小号字。 
<strong> 定义加重语气。 
<sub> 定义下标字。 
<sup> 定义上标字。 
<ins> 定义插入字。 
<del> 定义删除字。 

18.HTML CSS
A.改变字体和文字颜色
<html>

<head>
<style type="text/css">
h1 {color: red}
p {color: blue}
</style>
</head>

<body>
<h1>header 1</h1>
<p>A paragraph.</p>
</body>

</html>

B.隐藏链接下划线
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=gb2312" />
<meta http-equiv="Content-Language" content="zh-cn" />
</head>

<body>

<a href="/example/html/lastpage.html" style="text-decoration:none">
这是一个链接！
</a>

</body>
</html>

19.HTML链接
HTML 使用超级链接与网络上的另一个文档相连。
几乎可以在所有的网页中找到链接。点击链接可以从一张页面跳转到另一张页面。

A.创建超级链接
<p>
<a href="/index.html">本文本</a> 是一个指向本网站中的一个页面的链接。
</p>

<p>
<a href="http://www.microsoft.com/">本文本</a> 是一个指向万维网上的页面的链接。
</p>

B.使用图片作为链接
<p>
您也可以使用图像来作链接：
<a href="/example/html/lastpage.html">
<img border="0" src="/i/eg_buttonnext.gif" />
</a>
</p>

"链接文本" 不必一定是文本。图片或其他 HTML 元素都可以成为链接。

20.Target属性
使用 Target 属性，你可以定义被链接的文档在何处显示。
下面的这行会在新窗口打开文档：
<a href="http://www.w3school.com.cn/" target="_blank">Visit W3School!</a>

21.