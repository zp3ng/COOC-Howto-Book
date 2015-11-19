二、环境搭建并创建仓库
====
----

### 安装GitHub并建立仓库
1.打开[GitHub](https://github.com)创建GitHub账户   
![注册GitHub1](images/signup1.png)
![注册GitHub2](images/signup2.png)
2.在GitHub上建立一个远程仓库，仓库名规则：username.github.io（username为你的GitHub用户名）   
![创建仓库](images/create-reponsitory.png)
3.下载并安装[GitHub客户端](https://github-windows.s3.amazonaws.com/GitHubSetup.exe)   
4.打开GitHub客户端，输入之前注册的GitHub账号登录，配置你的GIT（此处输入你姓名拼音和你的邮箱），然后点击`dashboard`   
![登录](images/github_login.png)   
![配置Git](images/config_github.png)   
5.点击左上角的加号，选择`Create`，Name输入：`username.github.io（username为你的GitHub用户名）`，点击`Browse`   定位到“C:\User\电脑当前用户名” 这个文件夹，点击`Create reponsitory`，创建一个本地仓库完成。
![创建本地仓库](images/create_local_rep.png)


### 安装Jekyll
1.下载并安装最新的[Rubyinstaller](http://files.bryanbibat.net/rails-ftw-v0.21-2.1.6-4.2.3.exe)，注意！安装时勾选`Add Ruby executables to your PATH`，且安装路径不能包含空格。   
2.安装完成后从开始菜单打开`Start Command Prompt with Ruby`   
3.运行`gem sources`查看gem安装源列表   
4.运行`gem source -r 刚才看到的源`删除gem默认的官方源（因为官方源被墙）   
5.运行`gem source -a https://ruby.taobao.org`将官方源改成淘宝源   
6.运行`gem update system`更新一下gem   
7.运行`gem install jekyll`安装Jekyll（安装速度视网速而定，安装完成之后会有相应提示，请耐心等待）   
![安装Jekyll](images/jekyll_install.png)