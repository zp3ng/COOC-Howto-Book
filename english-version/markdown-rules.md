# 三、Basic markdown rules

---


## Basic symbol

* \*,-,+ they have the same function,and be named the Markdown symbol.

* The blank line indicates another paragraph


## Change the line
* Single paragraph (& lt;  & gt;) with a blank line

* Two consecutive spaces will become one &lt;br&gt(Line breaks);

* 3 consecutive symbols, followed by a blank line, indicating the hr horizontal line (a horizontal line)

## Title
* proceed h1--h6,you can add 1--6 #,for example,# First-level title,## Second-level title...

* Bold text is through the text around the two **

## Quotes
* Add ">" and a space on the first line to indicate the code reference, and can also be nested

## List
* using *,+,- and add a space to show a

* 可以支持嵌套

* 有序列表用数字+英文点+空格来表示


## 超链接
* 直接写 \[文本](你的链接地址)

* 引用 先定义 [ref_name]:url，然后在需要写入url的地方， 这样使用[文本][ref_name]，通常的ref_name一般用数字表示，这样显得专业

* 简写url：用尖括号包裹url 这样生成的url锚文本就是url本身

## 插入图片
* 一行表示: !\[alt_text](url "可选的title")

* 引用表示法: !\[alt_text](id),预先定义 [id]:url "可选title"

* 直接使用&lt;img&gt;标签，这样可以指定图片的大小尺寸

## 特殊符号
* 用'\'来转义，表示文本中的markdown符号

* 可以在文本种直接使用html标签，但是要注意在使用的时候，前后加上空行

* 文本前后各加一个符号，表示斜体



