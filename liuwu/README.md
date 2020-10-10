任务一
-----------
# 工具
**Git**
  
**Notepad++** 
   
~~VS code~~  
-----------
# 一、开始用git。
一开始就遇到了问题。  
教程：输入  
$ git config --global user.name "Your Name"  
$ git config --global user.email "email@example.com"  
我：  
iuwu5@▒▒▒▒▒▒ MINGW64 ~/Desktop/新建文件夹 (2)/learngit (master)
$ git config --global user.name "iuwu5"  
iuwu5@▒▒▒▒▒▒ MINGW64 ~/Desktop/新建文件夹 (2)/learngit (master)
$ git config --global user.email “40204814@qq.com"  
???这两个不应该连在一起吗？我开错应用了？？？  
后来我才知道我有多憨  
！[捂脸.jpg](C:\Users\刘泽域\Desktop\README\README\捂脸.jpg)  
  
之后在网上看的说TortoiseGit好用，我就去下了一个，下好后弹了好几个窗口，之后Git就不能用了，删了TortoiseGit也不行，我就把Git删了重下了一个  
然后  
#### 什么都没有了
我人傻了  
# 二、用VS code。
在b站上找到了一个用VS code写Git的教程，我之前有用过VS code就试了下，不得不说，VS code真好用。  
但总是出现问题  
PS C:\Users\刘泽域\Desktop\gitdemo> git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/iuwu5/gitdemo.git'  
传不上去，我再查，好像是不在master的支上，就用了网上给的几个代码：  
PS C:\Users\刘泽域\Desktop\gitdemo> git remote add origin https://github.com/iuwu5/gitdemo.git  
fatal: remote origin already exists.

PS C:\Users\刘泽域\Desktop\gitdemo>  git pull origin master    #git pull --rebase origin master  
fatal: couldn't find remote ref master  

**fatal**  **fatal**  **fatal**  我......有没有点新鲜的？    
  
  
PS C:\Users\刘泽域\Desktop\gitdemo> git push -u origin master -f
Logon failed, use ctrl+c to cancel basic credential prompt.
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (7/7), 501 bytes | 250.00 KiB/s, done.
Total 7 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/iuwu5/gitdemo.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.  
**ohhhhhhhhhhh!!!**  
但网上说这种加了 -f 的代码可能会导致代码丢失，我也不知道怎么处理，我就回去用Git了。


# 三、体会。  
1、熟能生巧，“git init” “git add” “git commit -m “”” “git status”这几个代码我这几天不知打了多少遍，我现在闭上眼都可以把这几个打出来。
2、耐心，我在网上找的教程几乎每个都和我不太一样，明明是一样的步骤，他动下我动下，可就不一样，就现在的这个东西我也是写了两遍，我们无论遇到什么困难，都不要怕，冷静着去面对他。  
3、百度是个好东西，但要甄别，有好多陈年老货或是错的课程，我就去找一样的、好的的地方学。  



标题
---------------------------
# 1级标题 
## 2级标题
### 3级标题
#### 四级标题 
##### 五级标题  
###### 六级标题

文本样式
---------------------------
*强调文本* _强调文本_
**加粗文本** __加粗文本__
==标记文本==
~~删除文本~~
> 引用文本
>>H~2~O is是液体。
>>>2^10^ 运算结果是 1024。

列表
---------------------------
- 项目
  * 项目
    + 项目

1. 项目1
2. 项目2
3. 项目3

- [ ] 计划任务
- [x] 完成任务


表格
---------------------------
项目     | Value
-------- | -----
电脑  | $1600
手机  | $12
导管  | $1

| Column 1 | Column 2      |
|:--------:| -------------:|
| centered 文本居中 | right-aligned 文本居右 |


自定义列表
---------------------------
Markdown
:  Text-to-HTML conversion tool

Authors
:  John
:  Luke


注脚
---------------------------
一个具有注脚的文本。[^1]

[^1]: 注脚的解释

注释
---------------------------
Markdown将文本转换为 HTML。

*[HTML]:   超文本标记语言  
  
# 四、进入程序部想学的东西
1、想在程序部里学习常用的语言。
2、多写点东西，练习技术。
3、找大佬问问题（这几天各种问题快把我整吐了）。
4、交一些志趣相同的朋友。