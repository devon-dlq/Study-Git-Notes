#### CREAT(创建)

> **git init**                    在当前目录下创建一个本(Create a new local repository)

> **git clone  ssh://user@domain.tld/repo.git**   在远程库克隆一个本地库(Clone an existing repository)

------

#### Configuration(配置)

> **git config [--global] user.name**    设置提交时附带的名字(Set the name attached to all your commits)

> **git config [--global] user.email**     设置提交时附带的email(Set the email attached to all your commits)

> **git config --global color.ui auto**     设置命令行输出回执的颜色(Set colorzition of  command line output for all repos)

> **git config [--global] user.name**      获取当前库设置的用户名(Print set name(in current repository or globally))

> **git config [--global] user.email**      获取当前库设置的email(Print set email(in current repository or  globally))

------

#### Local Changes(本地操作)

> **git status**    查看工作区内的文件修改(List changed files in your working directory)

> **git diff**     查看已追踪文件的修改(List changed to tracked files)

> **git add**     添加此文件的所有修改在下次提交时(Add all current changed in file to the next commit)

> **git add .**    添加本地库中的所有修改在下次提交的时(Add all current changed to the next commit)

> **git mv**      修改文件名并添加到下次提交当中(Rename file and add it to next commit)

> **git rm**      删除此文件并将此处删除添加到下次提交当中(Delete file and add its deletion to next commit)   

> **git commit -a**      提交工作区所有文件(Commit all local changes in tracked files)

------

#### Commit History(提交历史)

> **git log**                        显示所有的提交日志(Show all commits)

> **git log -p**                    这个文件的最后一次提交日志(Shwo changes over time for a specific file)

> **git log --author=<committer name>**  这个提交者最后一次的提交日志(Show changes over time for a specific committer)

> **git blame <file>**                此文件被谁修改了(Who changed what and when in file)

> **git stash**                      查看临时的文件变动 (Store changes temporarily)

> **git stash pop**                   删除上一次记录储蓄新的改动记录(Remove and apply changes)

> **git rm --cached <file>**           把此文件从过去的提交记录中删除但是保留当前本地的文件(Remvoe file from previous commits but keep it locally)

------

#### Branches & Tags(分支和标签)

> **git branch**                 本地所有的分支列表(List all existing branches)

> **git checkout <branch>**       切换分支(Switch HEAD branch)

> **git branch <new branch>**     创建新分支(Creat a new branch based on your current HEAD)

> **git branch --track <new-branch><remote-branch>**  创建一个新的分支基于一个远程的分支(Creat a new  tracking branch based on a remote branch)

> **git branch -d <branch>**              删除一个本地分支(Delete a local branch)

> **git branch origin --delete <branch>**    删除一个远程分支(Delete a remote branch)

> **git push <remote> : <old name>**   重命名远程分支名(Rename a branch on remote)git push
>
>  **git push <remote> <new name>**      

> **git tag <tag-name>**    给当前提交打一个tag,也可以查看当前标签(Tag the current commit)

------

#### Update & Publish(更新和提交)

> **git remote -v**              查看远程库的地址列表(List all currently configured remotes)

> **git remote show <remote>**    查看这个远程库的信息(Show information about a remote)

> **git remote add <remote> <url>** 添加新的远程库(Add new remote repository)

> **git remote rename <old-name> <new-name>**    重命名远程库(Rename a remote)

> **git fetch <remote>**     从远程库更新所有的信息到本地，但是不合并(Download all changes from remote,but don't merge into HEAD)

> **git fetch -p <remote>**    从远程库更新所有的信息到本地，但是不合并并清理已删除的远程分支(Download all changes fromm remote,but don't merge in HEAD and clean up deleted branchs from origin)

> **git pull <remote><branch>**  从远程库更新数据并立即合并数据(Download changes and directly merge into HEAD)

> **git push <remote><branch>**   将本地数据同步到远程库中(Publish local changes on a remote)

> **git remote add --track <remote-branch><remote><url>**  追踪一个远程库(Track a remote repository)

> **git push --tags**             同步标签到远程库(Publish your tags

> **git remote show <remote>**    显示远程库信息(Show information about a submodule)

------

#### Merge & Rebase(分支合并和重整数据)

> **git merge <branch>**    将其他分支和并到当前分支(Merge branch into your current HEAD)

> **git rebase <branch>**       将亲她分支合并到当前分支并按照提交顺序排序(Rebase your current HEAD onto branch)

> **git rebase --abort**        终止当前合并(Abort a rebase)

> **git rebase --continue**     解决冲突后继续当前合并和重整(Continue a rebase after resolving confilcys)

> **git mergetool**            使用配置的合并工具解决冲突(Resolve conflicts using your configured merge tool)

> **git add <resolved-file>**   手动解决冲突使用编辑器并标记已解决的文件
>
> **git rm <resolved-file>**

------

#### Undo(撤销)

> **git reset --hard HEAD**          丢弃所有的本地修改(Discard all local changes in your working directory)

> **git checkout HEAD <file>**      丢弃此文件的本地修改(Discard local changes in a specific file)

> **git revert  <commit>**          撤销某次的提交内容(Revert a commit by providing a new commit with contrary changes)

> **git checkout <commit><file>**   撤销某次提交的某个文件的内容(Revert a specific file from a previous commit)

------

#### 重置头指针到过去的某个提交上,版本回退(Reset your HEAD pointer to a previous commit)

> **git reset --hard  <commit>**    回退到某个版本(Discarding local changes)

> **git reset <commit>**           回退到某个版本并保存未追踪的改动

> **git reset --keep <commit>**    回退到某个版本并保存未提交的改动

