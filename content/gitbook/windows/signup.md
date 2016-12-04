# 四、创建书并关联Gitlab仓库

---

1.首先，你需要登陆[https://about.gitlab.com/gitlab-com/](https://about.gitlab.com/gitlab-com/)， 注册一个Gitlab账号,点击sign up或register按照提示注册即可，或者可以使用下方的关联账号进行授权登陆。

![](/assets/8000.png)  
2.需要创建一个Gitbook账号。登陆[https://www.gitbook.com/](http://www.gitbook.com/)， 点击下方的sign up进行注册，注册后进行登录。  
![picture113](/assets/图片3.png)  
也可以选择通过别的方式进行关联授权  
![picture114](/assets/图片4.png)  
3.我们进入Gitbook中，创建一本书，书的名字为test_book，Description里面写这本书的描述，填好后点击右下角的Create Book按钮  
![picture115](/assets/图片5.png)

4.这样一本书就创建好了，下面我们需要在Gitlab中导入这本书，首先我们需要知道这本书的地址，然后进入Gitlab的主界面，书的地址在Gitbook中获得，先进入我们创建的test_book这本书，然后:
![](/assets/8006.png)
然后我们在Gitlab主界面创建一个新的工程
![](/assets/8001.png)
工程内容如下：
![](/assets/8005.png)
点击导入后就会进入导入界面：
![](/assets/8007.png)
导入成功后就会显示这本书的内容：
![](/assets/8008.png)

5.这只是将工程导入了，现在需要把gitlab和gitbook关联起来，就是挂钩，这样我们只需要在gitbook上对内容进行修改，gitlab上的内容也会自动的进行同步：
首先在gitlab右侧的设置中找到Webhooks并进入：
![](/assets/8009.png)
进入Webhooks后，设置一些同步的内容：
![](/assets/8010.png)
导入完成后会在下方显示添加的这条Webhook：
![](/assets/8011.png)

6.建立了gitlab与gitbook的联系以后，我们就可以安静的写书了，首先我们需要下载Gitbook客户端，在客户端中用markdown编辑既方便又快捷，我们首先需要将我们在云端的test_book这本书下载到本地，编辑后再将test_book上传到云端，下载如下图所示：  
![picture120](/assets/图片10.png)  
7.进入这本书以后，就可以编辑了：  
![test8](/assets/test8.png)  
8.写完后同步到云端：  
![](/assets/8012.png)
9.同步后，就可以登陆gitbook和gitlab上，发现仓库中的内容发生了变化，所以我们以后就可以在Gitbook客户端上编写，然后上传到云端以网页的形式显示出来。  

**现在已经将GitBook上书的仓库和Gitlab上书的仓库关联起来了，以后既可以通过GitBook写书，也可以将更新提交到Gitlab，极大的方便了多人协作撰写一本课本。**

**以后就可以通过**[**https:\/\/username.gitbook.io\/仓库名\/**](https://username.gitbook.io/仓库名/)** 在线阅读或下载图书。**

_下面介绍通过GitBook客户端撰写的方法。_

