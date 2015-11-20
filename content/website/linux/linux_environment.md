环境搭建
===
---

### 创建GitHub账户
打开[GitHub](https://github.com)创建GitHub账户   
![注册GitHub1](../images/signup1.png)
![注册GitHub2](../images/signup2.png)


### 安装Git
在终端里，运行如下命令：

	$ sudo apt-get install git #安装Git
	$ git config --global user.name "Git用户名（随意取）"
	$ git config --global user.email "邮箱"

### 安装Ruby
Ubuntu 官方镜像的Ruby版本太低，需要先卸载自带的Ruby：

	$ sudo apt-get remove ruby

添加第三方源，安装新版本Ruby：

	$ sudo apt-get install python-software-properties
	$ sudo apt-add-repository ppa:brightbox/ruby-ng
	$ sudo apt-get update
	$ sudo apt-get install ruby2.2 ruby2.2-dev

### 安装Jekyll

	$ gem sources #产看Gem的源
	$ gem source -r 刚才看到的源 #删除gem默认的官方源（因为官方源被墙）
	$ gem source -a https://ruby.taobao.org #将官方源改成淘宝源
	$ gem update system #更新Gem
	$ sudo gem install jekyll