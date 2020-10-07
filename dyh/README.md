# 升华程序部2020招新任务一
# Git 学习
## 1. Git安装及环境变量配置
1. 在使用Git前需要将git安装在你的计算机上，在Windows上安装Git可以直接在Git官网下载。官网地址<https://git-scm.com/download/win>。
2. 设置用户名及地址  
    
        $ git config --global user.name "your name" 
    
        $ git config --global user.email “your email"
    配置文件的查看
    Users\\.gitconfig文件中查看  
    ![Git配置.png](https://i.loli.net/2020/10/06/4c7Q2VjGeuDw9P8.png)
3. 配置文本编译器  
     配置步骤：在编辑器的文件->首选项->设置->搜索git.path->点击编辑->找到你的电脑git的安装目录，找到里面的bin文件夹，里面的git.exe文件把该文件的完整路径复制下来
## 2.本地仓库搭建
创建本地仓库的方式有两种：  
1. 在当前目录下新建一个Git代码库
          
        $ git init
2. 克隆远程目录

        $ git clone [url]
## 3.Git 文件操作
### 文件4种状态
版本控制就是对文件的控制，要对文件进行修改，提交等操作，首先要知道文件当前所在状态  
+ **Untracked**：未跟踪，此文件在文件夹中，但没加入git库，不参与版本控制，通过`git add`状态变为`Staged`
+ **Unmodify**：文件已经入库，未修改，及版本库中的文件快照内容与文件夹中完全一致，这种类型的文件有两种去处，如果它被修改，变为`Modified`。如果使用`git rm`移处版本库，则成为`Untracked`文件
+ **Modified**：文件已修改，仅仅是修改，并无其他操作，此类文件也有两个去处，通过`git add` 可以进入暂存`Staged`状态，使用`git checkout`则丢弃修改结果，返回到`Unmodify`状态，`git checkout`即从库中取出文件，覆盖当前修改
+ **Staged**：暂存状态，执行`git commit`则将修改同步到库中，这时库中的文件和本地文件又变为一致，文件为`Unmodify`状态，执行`git reset HEAD filename`取消暂存，文件状态为`Modified`
## 4.git分支
列出所有的本地分支  
`git branch`
列出所有远程分支
`git branch -r`
新建一个分支但仍停留在当前分支`git branch [branch-name]`
新建一个分支并切换到该分支`git checkout -b [branch]`
合并指定分支到当前分支
`git merge[branch]`
## 5. 遇到的问题
配置ssh后仍需输入用户名密码

将http修改为Git@后问题解决
# markdown学习
