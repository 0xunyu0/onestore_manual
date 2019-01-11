>大神可以直接绕道了，这是给新手学习用的。

# markdown语法总结
## **1.1 区块元素**
## **1.1.1 区块引用**
引用标记符为>，通常用作标注文章的主旨，名人名言的引用等
``` example
>这是一个引用（上下都要回车占位!!!）

>这是一个引用
```
>这是一个引用

>这是一个引用

区块引用可以嵌套（例如：引用内的引用），只要根据层次加上不同数量的 > 
``` example
>
> > This is nested blockquote.
>
> Back to the first level.
```
>
> > This is nested blockquote.
>
> Back to the first level.

引用的区块内也可以使用其他的 Markdown 语法，包括标题、列表、代码区块等
``` example
> ## 这是一个标题。
> 
> 1.   这是第一行列表项。
> 2.   这是第二行列表项。
> 
> 给出一些例子代码：
> 
>     return shell_exec("echo $input | $markdown_script");
```

> ### 这是一个标题。
> 
> 1.   这是第一行列表项。
> 2.   这是第二行列表项。
> 
> 给出一些例子代码：
> 
>     return shell_exec("echo $input | $markdown_script");

## **1.1.2 标题**

``` example
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
**粗体字**
__粗体__
*斜体*
_斜体_
~~文字删除线~~
最高阶标题（上下都要回车占位）
==========================

第二阶标题（上下都要回车占位）
--------------------------
```
**粗体字**
__粗体__
*斜体*
_斜体_
~~文字删除线~~

## **1.1.3 段落和换行**
一个 Markdown 段落是由一个或多个连续的文本行组成，它的前后要有一个以上的空行（空行的定义是显示上看起来像是空的，便会被视为空行。比方说，若某一行只包含空格和制表符，则该行也会被视为空行）。普通段落不该用空格或制表符来缩进。
## **1.1.4 表格**
``` example
<table>
    <tr>
        <td>这是一个普通段落。</td>
      	<td>这是普通段落。</td>
    </tr>
    <tr>
        <td>这是普通段落。</td>
      	<td>这是一个普通段落。</td>
    </tr>
</table>

```

<table>
    <tr>
        <td>这是一个普通段落。</td>
      	<td>这是普通段落。</td>
    </tr>
  	<tr>
        <td>这是普通段落。</td>
      	<td>这是一个普通段落。</td>
    </tr>
</table>

``` table
| ABCD | EFGH | IJKL |
| -----|:----:| ----:|
| a    | b    | c    |
| d    | e    |  f   |
| g    | h    |   i  |

ABCD | EFGH | IGKL
-----|------|----
a    | b    | c
d    | e    | f
g    | h    | i
```


| ABCD | EFGH | IJKL |
| -----|:----:| ----:|
| a    | b    | c    |
| d    | e    |  f   |
| g    | h    |   i  |

ABCD | EFGH | IGKL
-----|------|----
a    | b    | c
d    | e    | f
g    | h    | i


## **1.1.5 列表**
**Markdown 支持有序列表和无序列表。**

**无序列表使用星号、加号或是减号作为列表标记：**
``` example
*   Red
*   Green
*   Blue

等同于：

+   Red
+   Green
+   Blue

也等同于：

-   Red
-   Green
-   Blue
```

*   Red
*   Green
*   Blue

等同于：

+   Red
+   Green
+   Blue

也等同于：

-   Red
-   Green
-   Blue

**有序列表则使用数字接着一个英文句点：**
```example

1.  Bird
2.  McHale
3.  Parish

```

1.  Bird
2.  McHale
3.  Parish

**很重要的一点是，你在列表标记上使用的数字并不会影响输出的 HTML 结果，上面的列表所产生的 HTML 标记为：**
``` example
<ol>
<li>Bird</li>
<li>McHale</li>
<li>Parish</li>
</ol>
```
**如果你的列表标记写成：**
```

1.  Bird
1.  McHale
1.  Parish

```
**或甚至是：**
```

3. Bird
1. McHale
8. Parish

```
**你都会得到完全相同的 HTML 输出。重点在于，你可以让 Markdown 文件的列表数字和输出的结果相同，或是你懒一点，你可以完全不用在意数字的正确性。**

如果你使用懒惰的写法，建议第一个项目最好还是从 1. 开始，因为 Markdown 未来可能会支持有序列表的 start 属性。

列表项目标记通常是放在最左边，但是其实也可以缩进，最多 3 个空格，项目标记后面则一定要接着至少一个空格或制表符。

要让列表看起来更漂亮，你可以把内容用固定的缩进整理好：
``` example
*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
    viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
    Suspendisse id sem consectetuer libero luctus adipiscing.
```

*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
    viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
    Suspendisse id sem consectetuer libero luctus adipiscing.
    
但是如果你懒，那也行：
``` example
*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
Suspendisse id sem consectetuer libero luctus adipiscing.
```
*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
Suspendisse id sem consectetuer libero luctus adipiscing.

如果列表项目间用空行分开，在输出 HTML 时 Markdown 就会将项目内容用 <p> 标签包起来，举例来说：

    *   Bird
    *   Magic
  
会被转换为：
  

    <ul>
    <li>Bird</li>
    <li>Magic</li>
    </ul>


但是这个：

``` mark
*   Bird

*   Magic
```
会被转换为：

``` html
<ul>
<li><p>Bird</p></li>
<li><p>Magic</p></li>
</ul>
```
列表项目可以包含多个段落，每个项目下的段落都必须缩进 4 个空格或是 1 个制表符：
``` example
1.  This is a list item with two paragraphs. Lorem ipsum dolor
    sit amet, consectetuer adipiscing elit. Aliquam hendrerit
    mi posuere lectus.

    Vestibulum enim wisi, viverra nec, fringilla in, laoreet
    vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
    sit amet velit.

2.  Suspendisse id sem consectetuer libero luctus adipiscing.
```
1.  This is a list item with two paragraphs. Lorem ipsum dolor
    sit amet, consectetuer adipiscing elit. Aliquam hendrerit
    mi posuere lectus.

    Vestibulum enim wisi, viverra nec, fringilla in, laoreet
    vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
    sit amet velit.

2.  Suspendisse id sem consectetuer libero luctus adipiscing.

如果你每行都有缩进，看起来会看好很多，当然，再次地，如果你很懒惰，Markdown 也允许：
``` example
*   This is a list item with two paragraphs.

    This is the second paragraph in the list item. You're
    
only required to indent the first line. Lorem ipsum dolor
sit amet, consectetuer adipiscing elit.

*   Another item in the same list.
```
*   This is a list item with two paragraphs.

    This is the second paragraph in the list item. You're
    
only required to indent the first line. Lorem ipsum dolor
sit amet, consectetuer adipiscing elit.

*   Another item in the same list.

如果要在列表项目内放进引用，那 > 就需要缩进：
``` example
*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.
```
*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.
    
如果要放代码区块的话，该区块就需要缩进两次，也就是 8 个空格或是 2 个制表符：
``` example
*   一列表项包含一个列表区块：

        <代码写在这>
```
*   一列表项包含一个列表区块：

        <代码写在这>
        
当然，项目列表很可能会不小心产生，像是下面这样的写法
``` example
1986. What a great season.
```
1986. What a great season.

换句话说，也就是在行首出现数字-句点-空白，要避免这样的状况，你可以在句点前面加上反斜杠。
``` example
1986\. What a great season.
```
1986\. What a great season.

## **1.1.6 分隔线**
你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：
``` example
* * *

***

*****

- - -

---------------------------------------
```
* * *

***

*****

- - -

---------------------------------------

## **1.1.7 代码区块**
要在 Markdown 中建立代码区块很简单，只要简单地缩进 4 个空格或是 1 个制表符就可以
``` example
Markdown 会用 <pre>与<code>标签来把代码区块包起来。
<pre><code>这是一个代码区块。
</code></pre>
```
<pre><code>这是一个代码区块。
</code></pre>

一个代码区块会一直持续到没有缩进的那一行（或是文件结尾）所以请注意回车换行。

## **1.2 区段元素**
## **1.2.1 链接**
Markdown 支持两种形式的链接语法： **行内式**和**参考式**两种形式。

不管是哪一种，链接文字都是用[方括号]来标记。

**行内式的链接**，只要在方块括号后面紧接着圆括号并插入网址链接即可，如果你还想要加上链接的 title 文字，只要在网址后面，用双引号把 title 文字包起来即可，例如：
``` example
[an example](http://example.com/ "Title") This is inline link.

[This link](http://example.net/) has no title attribute.
```

[an example](http://example.com/ "Title") This is inline link.

[This link](http://example.net/) has no title attribute.

如果你是要链接到同一主机的资源，你可以使用相对路径：
``` example代码
[About](/about/) See my page for details.
```
[About](/about/) See my page for details.

**参考式的链接**是在链接文字的括号后面再接上另一个方括号，而在第二个方括号里面要填入用以辨识链接的标记：
``` example代码
[an example][id] This is reference-style link.
你也可以选择性地在两个方括号中间加上一个空格：
[an example] [id] This is reference-style link.
接着，在文件的任意处，你可以把这个标记的链接内容定义出来：
[id]: http://example.com/  "Optional Title Here"
这个标记的链接内容的其他写法
[id]: http://example.com/  'Optional Title Here'   或
[id]: http://example.com/  (Optional Title Here)
```
[an example][id] This is reference-style link.

[id]: http://example.com/  "Optional Title Here" 

链接的定义可以放在文件中的任何一个地方，我比较偏好直接放在链接出现段落的后面，你也可以把它放在文件最后面，就像是注解一样。

下面是一个参考式链接的范例：
``` example代码
I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"
```
I get 10 times more traffic from [Google] [1] than from
[Baidu] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://www.baidu.com/  "Baidu Search"
  [3]: http://search.msn.com/    "MSN Search"

## **1.2.2 强调**
Markdown 使用星号（*）和底线（_）作为标记强调字词的符号
``` example代码
*single asterisks*

_single underscores_

**double asterisks**

__double underscores__
```
*single asterisks*

_single underscores_

**double asterisks**

__double underscores__


## **1.2.3 代码**

## **1.2.4 图片**
很明显地，要在纯文字应用中设计一个「自然」的语法来插入图片是有一定难度的。

Markdown 使用一种和链接很相似的语法来标记图片，同样也允许两种样式： 行内式和参考式。

**行内式**的图片语法看起来像是：
``` example代码
![Alt text](/path/to/img.jpg)

![Alt text](/path/to/img.jpg "Optional title")
```
详细叙述如下：
一个惊叹号 !
接着一个方括号，里面放上图片的替代文字
接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上 选择性的 'title' 文字。

**参考式**的图片语法则长得像这样：
``` example代码
![Alt text][id]
「id」是图片参考的名称，图片参考的定义方式则和链接参考一样：

[id]: url/to/image  "Optional title attribute"

到目前为止， Markdown 还没有办法指定图片的宽高，如果你需要的话，你可以使用普通的 <img> 标签。
```
## **1.3 更多收集**

## **1.3.1 反斜杠**