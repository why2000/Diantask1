# 了解Git的概念、原理和使用方法

[Day3]

* * *

## 本日进度

### 1. 在 [推荐！手把手教你使用Git - 文章 - 伯乐在线](http://blog.jobbole.com/78960/) 中学习了基本git指令的使用。

1. 版本库的创建(git init)
2. 文件提交到暂存区与上传至分支
3. 版本的回滚与选择(git reset, git checkout)
4. 历史版本的查看(git reflog/git log)
5. 版本修改详细信息的查看(git diff)

### 2. 通过学习 [git reset soft,hard,mixed之区别深解 - 世有因果知因索果 - 博客园](https://www.cnblogs.com/kidsitcn/p/4513297.html) 以及 [创建与合并分支 - 廖雪峰的官方网站](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/001375840038939c291467cc7c747b1810aab2fb8863508000)加深了对于git版本控制的理解

> HEAD: 顶端版本(最近一次commit)  
>
> INDEX: 当前的暂存区(最近一次add)  
>
> WORKING COPY: 目前你的文件本身的样子(最近一次保存文件本身)  
>
> master/dev: 各个不同的分支，用于被HEAD等所指向  
>
> `branch` 从当前位置创建分支，后跟分支名  
> + 添加参数 `-d` 表示删除该分支  
>
> `checkout`: 使HEAD指向对应参数，可以是某个commit，也可以是一个分支。  
> + 但不改变当前分支顶点，会使HEAD与当前分支顶点分离。  
> + 添加参数 `-b` 表示创建并checkout到创建的分支
>
> `reset`: 把HEAD和其当前所指的分支顶点(如果存在)移动到指定位置  
> + `--hard`: 带上了INDEX和WC一起动  
> + `--soft`: 只动HEAD  
> + `--mixed`: 带上INDEX一起动  
>
> `merge`: 将指定分支合并到当前分支(在没有冲突的情况下)  
> + 添加参数 `--no-ff` 后，用 `branch -d` 删除分支后仍保留分支的信息
>

### 3. 学习了如何在本地git库与远程仓库间进行传输。

1. 生成/查看本地SSH密钥  
> + `cd ~/.ssh`
> + `ssh-keygen -t rsa -C "email@email.com"`

2. 在本地库添加远程仓库，并在远程仓库添加SSH公钥
> + `git remote add origin https://mygit.com/git1.git`

3. 推送到远程库
> + `git push -u origin master`(第一次时用此命令，以后用下面一个)
> + `git push origin master`

4. 从远程库导入
> + `git clone https://mygit.com/git2`

* * *

[Day4]

* * *

## 本日进度

### 继续使用Git Bash练习了目前掌握的git基本语法，对分支控制有了进一步的理解

> 注: 如果你已经打开了这份笔记，应该已经知道了我的github地址: [why2000 (伍瀚缘)](https://github.com/why2000)(https://github.com/why2000)