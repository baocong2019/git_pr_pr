# git command

[Git在线练习教程网址](https://learngitbranching.js.org/?demo=&locale=zh_CN)

0.git add.

添加所有改动到暂存区（INDEX）    .代表所有文件

1.git commit -m "commit message"

提交新的改动到本地仓库

2.git push origin master

推送本地仓库到远程仓库

2.1.git pull origin master

拉取远程仓库的最新改动到本地仓库

3.git branch <branch-name>

创建新分支  <branch-name>为新分支的名称 不需要带<>这个符号，直接打分支名称即可 

branch: 分支

4.git checkout <branch-name>

**checkout: 检验**

切换到指定分支

5.git merge <branch-name>

合并指定分支到当前分支  

**merge: 融合，合并**

6.git rebase <branch-name>

，将当前分支合并到指定分支

第二种合并分支的方法是 git rebase。Rebase 实际上就是取出一系列的提交记录，“复制”它们，然后在另外一个地方逐个的放下去。Rebase 的优势就是可以创造更线性的提交历史，这听上去有些难以理解。如果只允许使用 Rebase 的话，代码库的提交历史将会变得异常清晰。

7.git checkout HEAD^

向上移动到上一个版本    首先看看操作符 (^)。把这个符号加在引用名称的后面，表示让 Git 寻找指定提交记录的 parent 提交。
使用 ~<num> 向上移动多个提交记录，如 ~3 向上移动三次。

8.git branch -f <branch-name> <commit-id>

强制覆盖本地分支，将指定提交记录作为新分支的起点。
例子：git branch -f bugFix HEAD~3 代表的意思是：将 HEAD 指向的提交记录移动向前三次，作为 bugFix 分支的起点。
