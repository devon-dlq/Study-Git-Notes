# git学习笔记

#### 新建仓库

```
在当前目录新建Git代码库
git init

新建一个目录，并将它初始化为Git代码库
git init [project-name]

从GitHub下载一个项目和整个代码历史
git clone [url]
[url] 为项目的地址
```

#### 提交

```
添加一个或多个文件到缓存区
git add file-name

添加指定目录到缓存区
git add [dir]

添加当前目录下所有文件到缓存区
git add .

查看在你上次提交之后是否有对文件进行再次修改。
git status (通常使用 -s 参数来获得简短的输出结果)

将暂存区内容添加到本地仓库中
git commit -m [message]  ([message]  可以是备注信息)

提交暂存区的指定文件到仓库区
git commit [file] ... -m [message]

-a 参数设置修改文件后不需要执行 git add 命令，直接来提交
git commit -a

将本地的分支版本上传到远程并合并。
git push <远程主机名> <本地分支名>:<远程分支名>

将本地的 master 分支推送到 origin 主机的 master 分支
git push origin master(master具体为实际分支)

如果本地版本与远程版本有差异，但又要强制推送可以使用 --force 参数：
git push --force origin master

删除主机的分支可以使用 --delete 参数，以下命令表示删除 origin 主机的 master 分支：
git push origin --delete master
```

 #### 分支管理

```
创建分支命令：
git branch (branchname)

切换分支命令:
git checkout (branchname)
当你切换分支的时候，Git 会用该分支的最后提交的快照替换你的工作目录的内容， 所以多个分支不需要多个目录。

合并分支命令:
git merge 

列出分支基本命令：
git branch

没有参数时，git branch 会列出你在本地的分支。
$ git branch
* master

删除分支命令：
git branch -d (branchname)

将任何分支合并到当前分支中去：
git merge
```

$$x^{y^z}=(1+{\rm e}^x)^{-2xy^w}$$

 
