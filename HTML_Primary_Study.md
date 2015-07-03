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

21.Name属性——规定锚 实现页面内部跳转
name 属性规定锚（anchor）的名称。
您可以使用 name 属性创建 HTML 页面中的书签。
书签不会以任何特殊方式显示，它对读者是不可见的。
当使用命名锚（named anchors）时，我们可以创建直接跳至该命名锚（比如页面中某个小节）的链接，这样使用者就无需不停地滚动页面来寻找他们需要的信息了。
<a name="label">锚（显示在页面上的文本）</a>

可以看做是一种页面内部的链接跳转

#实例

首先，我们在 HTML 文档中对锚进行命名（创建一个书签）：
<a name="tips">基本的注意事项 - 有用的提示</a>

然后，我们在同一个文档中创建指向该锚的链接：
<a href="#tips">有用的提示</a>

您也可以在其他页面中创建指向该锚的链接：
<a href="http://www.w3school.com.cn/html/html_links.asp#tips">有用的提示</a>

在上面的代码中，我们将 # 符号和锚名称添加到 URL 的末端，就可以直接链接到 tips 这个命名锚了。

22.图像
<img src="url" />

A.替换文本属性
alt 属性用来为图像定义一串预备的可替换的文本。替换文本属性的值是用户定义的。
<img src="boat.gif" alt="Big Boat">
在浏览器无法载入图像时，替换文本属性告诉读者她们失去的信息

B。网页背景图片
<body background="/i/eg_background.jpg">
如果图片小于页面，图片会进行重复

C.图片排列
<p>图像 <img src="/i/eg_cute.gif" align="bottom"> 在文本中</p>
<p>图像 <img src ="/i/eg_cute.gif" align="middle"> 在文本中</p>
<p>图像 <img src ="/i/eg_cute.gif" align="top"> 在文本中</p>
<p>请注意，bottom 对齐方式是默认的对齐方式。</p>

D.浮动图像
<p>
<img src ="/i/eg_cute.gif" align ="left"> 
带有图像的一个段落。图像的 align 属性设置为 "left"。图像将浮动到文本的左侧。
</p>
<p>
<img src ="/i/eg_cute.gif" align ="right"> 
带有图像的一个段落。图像的 align 属性设置为 "right"。图像将浮动到文本的右侧。
</p>

E.调整图像大小
<img src="/i/eg_mouse.jpg" width="50" height="50">
<br />
<img src="/i/eg_mouse.jpg" width="100" height="100">
<br />
<img src="/i/eg_mouse.jpg" width="200" height="200">

F.制作图像链接
<a href="/example/html/lastpage.html">
<img border="0" src="/i/eg_buttonnext.gif" />
</a>

G.制作图像映射
指定图片区域，并且附上超链

H.制作图片映射
<a href="/example/html/html_ismap.html">
<img src="/i/eg_planets.jpg" ismap />
</a>

<img> 定义图像。 
<map> 定义图像地图。 
<area> 定义图像地图中的可点击区域。 

23.表格
每个表格由 table 标签开始。
每个表格行由 tr 标签开始。
每个表格数据由 td 标签开始。
<table border="1">
<tr>
  <td>100</td>
  <td>200</td>
  <td>300</td>
</tr>
<tr>
  <td>400</td>
  <td>500</td>
  <td>600</td>
</tr>
</table

A.边框
<table border="1">数字指定了表格的边框种类

B.表头
<th>Heading</th>
<th>Another Heading</th>
大多数浏览器会把表头显示为粗体居中的文本

C.空单元格
<td>&nbsp;</td>
如果直接为空，会影响表格的边框显示

<table> 定义表格 
<caption> 定义表格标题。 
<th> 定义表格的表头。 
<tr> 定义表格的行。 
<td> 定义表格单元。 
<thead> 定义表格的页眉。 
<tbody> 定义表格的主体。 
<tfoot> 定义表格的页脚。 
<col> 定义用于表格列的属性。 
<colgroup> 定义表格列的组。 

D.多列多行表头
<th colspan="2"></th>横跨两列的表头
<th rowspan="2"></th>横跨两行的表头

<table border="1">
<tr>
  <th>姓名</th>
  <th colspan="2">电话</th>
</tr>
<tr>
  <td>Bill Gates</td>
  <td>555 77 854</td>
  <td>555 77 855</td>
</tr>
</table>

<table border="1">
<tr>
  <th>姓名</th>
  <td>Bill Gates</td>
</tr>
<tr>
  <th rowspan="2">电话</th>
  <td>555 77 854</td>
</tr>
<tr>
  <td>555 77 855</td>
</tr>
</table>

E.居中对齐
<h4>带有 cellpadding：</h4>
<table border="1" 
cellpadding="10">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>   
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

<h4>带有 cellspacing：</h4>
<table border="1" 
cellspacing="10">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>   
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

F.颜色和背景
<h4>背景颜色：</h4>
<table border="1" 
bgcolor="red">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>   
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

<h4>背景图像：</h4>
<table border="1" 
background="/i/eg_bg_07.gif">
<tr>
  <td>First</td>
  <td>Row</td>
</tr>   
<tr>
  <td>Second</td>
  <td>Row</td>
</tr>
</table>

不同的背景颜色
<h4>单元背景：</h4>  
<table border="1">
<tr>
  <td bgcolor="red">First</td>
  <td>Row</td>
</tr>   
<tr>
  <td 
  background="/i/eg_bg_07.gif">
  Second</td>
  <td>Row</td>
</tr>
</table>

G.表格宽度和居左居右设置
<table width="400" border="1">
 <tr>
  <th align="left">消费项目....</th>
  <th align="right">一月</th>
  <th align="right">二月</th>
 </tr>
 <tr>
  <td align="left">衣服</td>
  <td align="right">$241.10</td>
  <td align="right">$50.20</td>
 </tr>
 <tr>
  <td align="left">化妆品</td>
  <td align="right">$30.00</td>
  <td align="right">$44.45</td>
 </tr>
 <tr>
  <td align="left">食物</td>
  <td align="right">$730.40</td>
  <td align="right">$650.00</td>
 </tr>
 <tr>
  <th align="left">总计</th>
  <th align="right">$1001.50</th>
  <th align="right">$744.65</th>
 </tr>
</table>

24.列表
A.无序列表
<h4>一个无序列表：</h4>
<ul>
  <li>咖啡</li>
  <li>茶</li>
  <li>牛奶</li>
</ul>

B.有序列表——列表元素前面会有序号显示
<ol>
  <li>咖啡</li>
  <li>牛奶</li>
  <li>茶</li>
</ol>

<ol start="50">
  <li>咖啡</li>
  <li>牛奶</li>
  <li>茶</li>
</ol>
 
C.自定义列表
<dl>
<dt>Coffee</dt>
<dd>Black hot drink</dd>
<dt>Milk</dt>
<dd>White cold drink</dd>
</dl>

<ol> 定义有序列表。 
<ul> 定义无序列表。 
<li> 定义列表项。 
<dl> 定义定义列表。 
<dt> 定义定义项目。 
<dd> 定义定义的描述。 

