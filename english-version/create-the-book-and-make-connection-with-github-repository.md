# Chapter 4:Create the book and make connection with Github repository

---

1.First,you need to log in [http://github.com/](https://github.com/),sign up a new Github account,click sign up and then follow the steps.

![picture112](/assets/图片2.png)
2.If you have the Github account,you don't need to sign up for a  new Gitbook account.[https://www.gitbook.com/](http://www.gitbook.com/),Click the "sign up" button on the top right corner.
![picture113](/assets/图片3.png)
choose sign in with Github
![picture114](/assets/图片4.png)
3.After get into the gitbook,we create a book named "test_book",finish the description and then click "Create Book" button.
![picture115](/assets/图片5.png)
    
4.So we create a book,next we should connect with Github to realize collaborative function.We get into the book,click "settings",then copy the book address in the following picture,this address is used to pass the URL of this book to a repository in Github.
![picture116](/assets/图片6.png)

5.Go to the [https://github.com/new/import](https://github.com/new/import),then put the address to the Url box,and create a Github repository.So that Github can synchronize with Gitbook through this address.
![picture117](/assets/图片7.png)

6.Click the "Begin import" above,then enter your github account and password.

![test4](/assets/test4.png)

7.After import,the github can know the gitbook address.
![picture118](/assets/图片8.png)

8.However,we have to give Gitbook the Github address.So we get back to Gitbook,add the repository for Github，it is "test_repository" we create at the fifth step.This completes the two-way communication between Gitbook and Github.
![picture119](/assets/图片9.png)

9.This completes the association of gitbook and github,using gitbook to write a book is enough,so why connect it with github?This is because github can be collaborative,for example,one book can be written by many writers,xiaohui is writing the book,and at the same time,xiaoqiang is writing as well.So github can know when and where who change the book,and change where.What's more,github can set permissions,for example,xiaohui is the creater and owner of the book,he wants to invite xiaoqiang to edit the book,so he can give the permission to xiaoqiang,then xiaoqiang have the authority to write this book.As following:

每个仓库都可以选择合作人：

![picture122](/assets/图片12.png)
10.建立了github与gitbook的联系以后，我们就可以安静的写书了，首先我们需要下载Gitbook客户端，在客户端中用markdown编辑既方便又快捷，我们首先需要将我们在云端的test_book这本书下载到本地，编辑后再将test_book上传到云端，下载如下图所示：
![picture120](/assets/图片10.png)
11.进入这本书以后，就可以编辑了：
![test8](/assets/test8.png)
12.写完后同步到云端：
![test9](/assets/test9.png)
13.同步后，就可以登陆gitbook和github上，发现仓库中的内容发生了变化，所以我们以后就可以在Gitbook客户端上编写，然后上传到云端以网页的形式显示出来。
![picture121](/assets/图片11.png)
**现在已经将GitBook上书的仓库和GitHub上书的仓库关联起来了，以后既可以通过GitBook写书，也可以将更新提交到GitHub，极大的方便了多人协作撰写一本课本。**

**以后就可以通过**[**https:\/\/username.gitbook.io\/仓库名\/**](https://username.gitbook.io/仓库名/)** 在线阅读或下载图书。**

_下面介绍通过GitBook客户端撰写的方法。_

