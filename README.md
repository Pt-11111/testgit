'gittest' 

## 初次使用
## git config --global user.name "name"
## git config --global user.email "email"


## git init 将当前目录作为仓库
## git clone https://github.com/libgit2/libgit2 克隆网络仓库
.gitignore 为忽略文件

## git help <opt>
## git <opt> --help


## git add 文件名.后缀  （暂存）

##  git commit 文件名.后缀(提交)

## git status 查看修改文件状态

## git diff 找不同

## git log 修改记录


##  组合操作
## git commit 文件
## git add 文件
## git commit --amend 补充提交

## git mv oldfile newfile  重命名

## git reset HEAD 文件名.后缀 （取消暂存）
                             ⬇此处有一个空格
## git checkout -- 文件名.后缀  恢复未修改前状态  慎用

## 远程仓库
## ssh-keygen -t rsa -C "邮箱地址" 
## 到用户目录/.ssh/id_rsa.pub 复制后添加到github sshkey管理
## github 新建仓库
## git remote add <(name)> git@github.com:<用户名>/仓库名             关联远程仓库
## git push -u origin master                              推送到远程仓库 
## 第一次加-u 以后只要本地作了提交，就可以 git push origin master
## git remote -v 查看远程库信息
## git remote rm 库名 删除远程绑定关系


## 创建分支
## git checkout -b dev 
## 相当于以下两条命令
## git branch dev
## git checkout dev 

## git branch   查看分支情况
## 带 * 号的是当前分支
## 