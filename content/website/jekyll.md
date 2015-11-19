# 基于Jekyll自定义网站

## 1.什么是Jekyll   
Jekyll是一种简单的、适用于博客的、静态网站生成引擎。它使用一个模板目录作为网站布局的基础框架，支持Markdown、Textile等标记语言的解析，提供了模板、变量、插件等功能，最终生成一个完整的静态Web站点。说白了就是，只要安装Jekyll的规范和结构，不用写html，就可以生成网站。
## 2.本地环境搭建
 （1）下载最新的[Rubyinstaller](http://files.bryanbibat.net/rails-ftw-v0.21-2.1.6-4.2.3.exe)并安装，**注意！安装时选中`Add Ruby executables to your PATH`，安装路径不能包含空格`**。安装完成后按组合键`Win+R`，输入`cmd`打开Windows命令行程序，输入`gem update –system`升级`gem`。   
 （2）下载最新的[DevKit](https://github.com/oneclick/rubyinstaller/downloads/)，DevKit是windows平台下编译和使用本地C/C++扩展包的工具。它就是用来模拟Linux平台下的make,gcc,sh来进行编译。但是这个方法目前仅支持通过RubyInstaller安装的Ruby，并双击运行解压到C:\DevKit。然后打开终端cmd，输入下列命令进行安装`cd C:\DevKit ruby dk.rb init ruby dk.rb install`   
 （3）完成上面的准备就可以安装Jekyll了,因为Jekyll是用Ruby编写的,打开终端cmd，输入：`gem install Jekyll`，安装完成后使用如下命令检验是否安装成功：`jekyll -version`。   
 （4）安装Rdiscount，这个用来解析Markdown标记的包，使用如下命令：`gem install rdiscount`    
 （5）运行本地工程,cd 到工程目录，输入：jekyll new .，启动服务：`jekyll server`    
 启动服务后，我们可以通过[http://localhost:4000](http://localhost:4000)来访问看我们的本地网站，当然现在什么都没有，后面继续结合上面在Github上创建的网站完成最后的工作。

 ### 3.使用Git工具配合Jekyll 写课程站点
 （1）下载最新[GitHub客户端](https://github-windows.s3.amazonaws.com/GitHubSetup.exe)   
 （2）在Github上添加ssh-key       
 首先我们在我们的电脑上查看以下本地的ssh-key,打开命令行CMD，输入`ssh-keygen -t rsa -C “email@email.com”`    
 其中”email@email.com”是github账号，然后会提醒你输入key的名称，输入如id_rsa；    
 在C:\Documents and Settings\Administrator\下产生两个文件：id_rsa和id_rsa.pub；    
 点击我们的用户头像，进入settings    
 点击SSH keys,并添加一个SSH key    
 点击Add SSH key按钮     
 点击Add key提交     
 titile可以随意取，key的内容时步骤3中的id_rsa.pub的内容，直接复制过去就可以。    

### 4.上传课程到GitHub
（1）在cmd中输入：git init   
（2）在GitHub上建立一个空的仓库   
（3）在cmd中输入git add -A，完成后输入git commit -m "init"，完成后输入git push 仓库地址，可能会要求输入GitHub用户名和密码