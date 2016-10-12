# 五、fork别人的仓库，pull request

---

####我们知道github是开源的，因此你创建的一本书（一个仓库），网络上的任何人都是可以看到的，我们如果发现别人的代码有问题，或者想帮助别人一起出书，可以将别人的代码fork（拷贝到自己的github中）下来，改好后，给作者发送一个合并请求，如果作者发现你做的确实是对的，就可以合并你的内容，实现协同合作功能。

我们举一个老师让学生编写书籍的例子：
![picture123](/assets/图片13.png)

我们还以test_book这本书为例，这本书的创建过程我们已经在上一节中说过了，下面我们以**weixh121001**这个github账号来做学生：

+ fork刚才我们创建的test_repository仓库。
+ 下载个Gitbook客户端编书
+ 发出pull request申请

1.进入老师给的test_repository仓库地址，然后fork，“Fork”就是把一个别人的仓库复制到自己的帐户中来。

https://github.com/yinhang2/test_repository


![picture124](/assets/图片14.png)
2.下载并安装GitHub客户端：https://desktop.github.com

3.打开GitHub客户端，首次打开需登录并初始化，步骤如下
![picture125](/assets/图片15.png)

接下来的“Configure”和“Repositories”步骤全部 选择“Skip”

4.登陆成功后点击左上角的“+”，后选择“clone”，然后选中“test_repository”仓库，然后点击下面的“Clone test_repository”
![picture126](/assets/图片16.png)

5.接下来在弹出的对话框中选择仓库在电脑上保存的位置，请务必记住这个位置，然后确定，接下来等正在clone的页面消失即可关闭GitHub客户端。
![picture127](/assets/图片17.png)

6.进入自己的Gitbook客户端，点击左上角的“Import”，在弹出的对话框中选择刚才用GitHub客户端clone的test_repository文件夹并打开
![picture128](/assets/图片18.png)

7.此时test仓库便会出现在GitBook首页中，点击它并可以打开它完成相应作业

8.作业完成后先点击左上角“Save”，然后再点击Save右边出现的☁️按钮

![picture129](/assets/图片19.png)

9.在接下来弹出的对话框中输入GitHub的用户名和密码，后点击“Sync”，此时便将你的作业同步到你账户中的test_repository仓库了，接下来还要从你的仓库中发送pull request

10.打开GitHub，进入学生的test_repository仓库，然后点击“Pull requests”
![picture130](/assets/图片20.png)

11.点击右边的“New pull request”

12.点击“Create pull request”
![picture131](/assets/图片21.png)

13.在展开的页面中“Title”处填写作业完成的大概情况，在“Leave a comment”处填写详细，后点击下方的“Create pull request”，至此作业提交完成。
![picture132](/assets/图片22.png)

这时老师在Github上就会得到pull request信息，点击pull request，点进test仓库
![picture133](/assets/图片23.png)
这时老师看了下信息，如果可以合并，就点击绿色按钮 Merge pull request，也可以回复Comment
![picture134](/assets/图片24.png)


