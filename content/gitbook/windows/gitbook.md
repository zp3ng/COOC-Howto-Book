一、GitBook介绍
===
---

GitBook是一个命令行工具(node.js库)， 使用Github/Git创建漂亮的图书。 你可以看一些用它编写的图书的例子： [高效使用 Mac OS X](https://www.GitBook.com/book/prettyxw/mac-os-x-tricks/details). 你也可以很容易的通过[GitBook.io](https://www.gitbook.com)网站发布在线图书。完整的文档可以在[help.gitbook.com](help.gitbook.com)网站找到.   

#### 输出格式

GitBook可以产生下列类型的图书：

- **静态站点**：默认格式。创建一个完全交互式的静态网站，可以发布到GitHub Pages等网站。
- **eBook**：图书完成后可以使用它创建电子书，输出格式可以是 **PDF**, **ePub** 或 **MOBI**。

#### 图书结构

一本图书就是一个Git仓库， 至少包含两个文件: `README.md` 和 `SUMMARY.md`。

	README.md 是你图书的简介，它可以被自动地加入到最终的 summary 之中

	SUMMARY.md 定义了图书的目录。它应该包含章节的列表，以及它们的链接。

例如：

SUMMARY.md

<!-- lang:CSS -->
	# Summary
	This is the summary of my book.
	* [section 1](section1/README.md)
    	* [example 1](section1/example1.md)
	    * [example 2](section1/example2.md)
	* [section 2](section2/README.md)
    	* [example 1](section2/example1.md)
    注意：一级标题和二级标题的无序列表用“ +-*/ ”等符号表示，切记通篇写作最好使用一种特殊符号标记。一级标题与二级标题最好用二个空格或四个空格区分，无序列表的特殊符号与文本要用空格隔开。
不被 `SUMMARY.md` 包含的文件不会被 `GitBook` 处理.  