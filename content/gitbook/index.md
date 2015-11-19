#如何使用 GitBook

GitBook是一个命令行工具(node.js库)， 使用Github/Git创建漂亮的图书。 你可以看一些用它编写的图书的例子： [高效使用 Mac OS X](https://www.GitBook.com/book/prettyxw/mac-os-x-tricks/details). 你也可以很容易的通过[GitBook.io](https://www.gitbook.com)网站发布在线图书。完整的文档可以在[help.gitbook.com](help.gitbook.com)网站找到.

##安装配置 GitBook 环境

以 Mac OS 为例

###安装工具
----------

<!-- lang:bash-->
	$ brew install node
	$ npm install -g GitBook-cli
	
###获取代码
-------

<!-- lang:bash-->
	$ git clone #位于 github 上的网址
	$ cd *clone #下来的本地路径

###编译使用
-------

<!-- lang:bash -->
	$ gitbook serve # 启动本地 Web Server
	
##输出格式
-------
GitBook可以产生下列类型的图书：

- **静态站点**：默认格式。创建一个完全交互式的静态网站，可以发布到GitHub Pages等网站。
- **eBook**：图书完成后可以使用它创建电子书。创建命令: `GitBook ebook ./myrepo`。你需要安装 [ebook-convert](http://manual.calibre-ebook.com/cli/ebook-convert.html)。输出格式可以是 **PDF**, **ePub** 或 **MOBI**。

##图书结构
-------
一本图书就是一个Git repository， 至少包含两个文件: `README.md` 和 `SUMMARY.md`。

````README.md 是你图书的简介，它可以被自动地加入到最终的 summary 之中
````

```` SUMMARY.md 定义了图书的目录。它应该包含章节的列表，以及它们的链接。
````

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
    	  
不被 `SUMMARY.md` 包含的文件不会被 `GitBook` 处理.  
###多语言
-------
GitBook 支持使用多种语言编写图书. 每种语言应该是一个子目录，遵循正常gitbook格式， `LANGS.md`文件应该被放到repository的根文件夹，格式如下：

<!-- lang:CSS -->
	* [English](en/)
	* [French](fr/)
	* [Español](es/)
	
###词汇表
-------

允许你列出条目以及它们的定义。基于这些条目 `gitbook` 会自动创建一个索引，并在页面中加亮这些条目。

GLOSSARY.md 格式如下：

<!-- lang:CSS -->
	# term
	Definition for this term
	# Another term
	With it's definition, this can contain bold text and all other kinds of inline markup ...
  
###忽略文件和文件夹
-------
GitBook 读取 `.gitignore`, `.bookignore` 和 `.ignore` 得到需要忽略的文件/文件夹的列表。（文件的格式和 `.gitignore`一样）。

`.gitignore` 最佳实践是忽略build文件，这些文件来自 `node.js` (node_modules, ...) 和GitBook的build文件: `_book`，`*.epub`， `*.mobi` and `*.pdf`。

###封面
-------
大尺寸封面文件为: `/cover.jpg`.
尺寸为 `1800x2360`。 插件 [autocover](https://github.com/GitbookIO/plugin-autocover)可以自动创建一个文件.

小尺寸封面为: `/cover_small.jpg`。

###发布图书
-------
平台 [GitBook.com](www.gitbook.com) 就像"Heroku for books": 你可以在它上面创建图书 (公开的, 付费的, 或者私有的)， 并且使用 

<!-- lang:CSS -->
	git push 

就可以更新。

###插件
-------
插件可以扩展图书的功能。查看插件介绍 [GitbookIO/plugin](https://github.com/GitbookIO/plugin)来了解如何创建一个插件。

官方插件：