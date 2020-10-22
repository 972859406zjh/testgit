Git是分布式版本控制系统，所以需要填写用户名和邮箱作为一个标识。
.git目录是Git来跟踪管理版本的，一般不建议改动文件内容，否则git仓库会被破坏掉。
在本地的testgit仓库下（E:\git\testgit）运行命令：

git remote add origin https://github.com/18515592159zhu/testgit.git
git push -u origin master把本地库的内容推送到远程，使用 git push命令，实际上是把当前分支master推送到远程。
由于远程库是空的，我们第一次推送master分支时，加上了 –u参数，Git不但会把本地的master分支内容推送的远程
新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令。
推送成功后，可以立刻在github页面中看到远程库的内容已经和本地一模一样了。

从现在起，只要本地作了提交，就可以通过如下命令：git push origin master

测试版本回退

test
666