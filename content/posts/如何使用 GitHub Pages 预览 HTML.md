---
title: "使用 GitHub Pages 预览 HTML"
date: 2019-10-13T23:45:56+08:00
draft: true
---

# 使用 GitHub Pages 预览 HTML
1. 在现有目录中创建本地仓库
````
git init
````

2. 将有改动或新增的文件添加到暂存区中
````
 git add .
````

3. 将暂存区中的改动提交到本地仓库
````
 git commit -m 'message'
 或
 git commit -v
````
4. 创建远程仓库
   
    ![创建远程仓库1](/images/1.jpg)
    ![创建远程仓库2](/images/2.jpg)   

5. 将本地仓库与远程仓库进行关联
   
    ![本地仓库与远程仓库关联](/images/3.jpg)
    远程仓库创建成功后选择SSH协议，然后使用git remote add 将本地仓库和远程仓库进行关联
````
git remote add origin git@github.com:youranjianmuchang/courses07.git
````
6. 将本地仓库的内容推送到远程仓库
````
git push -u origin master
````
7. 推送成功后刷新远程仓库的页面后，点击settings
   
    ![点击settings](/images/4.png)

8. 将页面下拉到GitHub Pages部分，将None改为master branch

    ![设置settings](/images/5.jpg)

9. 之后页面会刷新，再次将页面下拉到GitHub Pages部分，这次会看到多了一个链接，点击链接即可看到想要预览的html页面

    ![点击链接预览](/images/6.jpg)
    如果发现页面不能正常访问，可以在浏览器的地址后面补上想要看到的html文件名称即可