# Chapter 5:Fork repositories and pull request

---

#### We know that the github is open source，so you create a book（a repository）,anyone can see it on the website.If you find some problems about other people's code or you want to help others edit the book.You can fork them to your own github，after some changes，Send a merge request to the author，if the author find you are right，he can merge your request to achieve collaborative cooperation function.

We can use the "test_book" as an emample,the creation of the book has teached in the previous section.Now the example is a teacher wants to create a book named "test_book",so he arranges the task to his students,for the safety,students should fork the repository.We use **yinhang2** as the "teacher" and use **weixh121001** as the student：

+ fork the test_repository
+ download Gitbook client and edit the book
+ pull request to the teacher

1.Get into the test_repository address，then fork，“Fork” is to copy someone else's repository to his own account.

https://github.com/yinhang2/test_repository


![picture124](/assets/图片14.png)
2.Download and install Github client：https://desktop.github.com

3.Open github client，log in and waiting for initialization,proceed as follows

The “Configure” and “Repositories” steps we choose to "Skip"

4.Click on the top left corner of the "+" after logging in，then click "clone",choose the "test_repository" repository，after that click “Clone test_repository”
![picture126](/assets/图片16.png)

5.Next, in the pop-up dialog box,select the location where the repository is saved on the computer.Be sure to remember this location.Then wait for the clone page to disappear to close the GitHub client.
![picture127](/assets/图片17.png)

6.Get into the Gitbook client,click on the top left corner“Import”，In the pop-up dialog box, select GitHub client clone test_repository folder just now and open![picture128](/assets/图片18.png)

7.At this point the test repository will appear in the GitBook home page,Click it and open it to complete the corresponding job

8.After fininshing the job,click on the top right corner of the“Save”，and then click ☁️ button.

9.Then in the dialog,fill in the github username and password,and click "Sync",at this time ,your job is synchronized in your "test_repository" repository,you need to pull request to the teacher from your repository.
10.Open GitHub，get into the student's "test_repository" repository, then click "Pull requests"
![picture130](/assets/图片20.png)

11.Click the right button "New pull request"


12.Click "Create pull request"
![picture131](/assets/图片21.png)

13.In the following page,write general information about your job,then click "Create pull request",the job commition is done.
![picture132](/assets/图片22.png)

Now the teacher will see the pull request information from Github,the teacher can click "pull request" into the "test_repository" repository.
![picture133](/assets/图片23.png)
The teacher see the information，if it can be merged,then click the green button "Merge pull request",and can also leave some comment.
![picture134](/assets/图片24.png)


