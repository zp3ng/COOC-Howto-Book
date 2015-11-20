四、创作课程
===
---

1.在本地仓库的_post文件夹中创建一个Markdown文件，命名规则为：`年-月-日-文件名（不能为中文）.md`，如：2015-11-19-github-jekyll-course.md   
2.在刚才创建的课程页面文件中加入以下头信息

    ---
    layout: post
    title:  "课程名，如：GitHub搭配Jekyll，创建COOC课程网站（以Windows平台为例）"
    date:   创建时间，格式为：2015-11-19 14:43:48 +0800
    ---

3.接下来就可以按Markdown语法自由书写课程内容了，[Markdown语法](http://wowubuntu.com/markdown/)    
4.写的过程中可以随时运行`jekyll serve`，然后通过 http://127.0.0.1:4000 预览网站效果，完成之后，按照**[第三章、初始化Jekyll文件夹](init.md)**中的第6步将增加或修改的内容再次提交到远程仓库中去。