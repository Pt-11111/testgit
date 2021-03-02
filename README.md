'gittest' 

## 初次使用
 git config --global user.name "name"

 git config --global user.email "email"

***

## git init 将当前目录作为仓库
 git clone https://github.com/libgit2/libgit2 克隆网络仓库

git clone -b 分支名 地址     指定分支

.gitignore 为忽略文件

***

## 获取帮助
 git help \<opt>

 git \<opt\> --help

***

## （暂存）
git add 文件名.后缀  

***

## (提交)
git commit 文件名.后缀

git commit -a

git commit -m "message"

***

## （取消暂存）
git reset HEAD 文件名.后缀 
## 恢复未修改前状态  慎用
               ⬇此处有一个空格
git checkout -- 文件名.后缀   注意文件名前面的--

## 查看修改文件状态
git status 

## 找不同
git diff 

## 修改记录
git log 

***

##  组合操作 补充提交
 git commit 文件

 git add 文件

 git commit --amend 

## 重命名
git mv oldfile newfile  



## 远程仓库
 ssh-keygen -t rsa -C "邮箱地址" 

 到/用户目录/.ssh/id_rsa.pub 复制后添加到github sshkey管理
## github 新建仓库后 关联本地到远程仓库
 git remote add <(name)> git@github.com:<用户名>/仓库名             
## 推送本地到远程仓库 
git push -u origin master                              
## 第一次加-u 以后只要本地作了提交，就可以 git push origin master
## 查看远程库信息
git remote -v 
## 删除远程绑定关系
git remote rm 库名 

## 重命名远程库
git remote rename oldname newname

## 创建分支
 git checkout -b dev  此种情况默认是master的分支

 git checkout -b 分支的分支 分支   这种是指定复制分支

## 相当于以下两条命令
 git branch dev

 git checkout dev 

## 查看分支情况
git branch   
 带 * 号的是当前分支

## git checkout master 切换到master分支后 执行：
git merge dev 合并分支

## 删除分支
git branch -d \<name\>  删除本地分支

git push 远程仓库名 --delete 分支名   删除远程分支


## 创建分支：
git branch \<name\>

## 切换分支：
git checkout \<name\>或者git switch \<name\>

## 创建+切换分支：
git checkout -b \<name\>或者git switch -c \<name\>

## 合并分支
合并分支时，如果可能，Git会用Fast forward模式，但这种模式下，删除分支后，会丢掉分支信息。

如果要强制禁用Fast forward模式，Git就会在merge时生成一个新的commit，这样，从分支历史上就可以看出分支信息。

git merge --no-ff -m "message" dev     dev向当前分支合并


## 保存工作现场  不暂存也不提交
git stash 

git stash list 查看工作现场

git stash pop 恢复现场的同时删除现场 

等于以下的组合

git stash apply  \<指定现场名\>

git stash drop 
