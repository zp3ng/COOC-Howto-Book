三、安装环境、写作
===
---

### 安装Git
在终端里，运行如下命令：

	$ sudo apt-get install git #安装Git
	$ git config --global user.name "Git用户名（随意取）"
	$ git config --global user.email "邮箱"

### 安装Nodejs
运行命令：

	$ curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash -
	$ sudo apt-get install -y nodejs

### 安装GitBook
运行命令：

	$ sudo npm install -g gitbook-cli

### 同步代码
	$ git clone GitHub仓库的地址

### 撰写
按照GitBook目录的说明创建章节等并撰写相关内容。

### 预览
在本地仓库根目录运行：
	$ gitbook serve
即可在浏览器中预览书的静态站点，也可以运行：
	$ gitbook pdf
生成PDF电子书，确认修改无误后运行：
	$ git add -A
	$ git commit -m "提交说明"
	$ git push origin master
将修改提交到远程仓库里去