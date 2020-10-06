# Git学习报告
土木工程国际2002班黄鹄

## Git是什么？
git就是课代表，你把作业给他，他帮你交作业。

## 课代表Git听得懂中文吗？

听不懂，人家只会international的english啦，使用Git的语法跟他打招呼啦。

## 如何向Git自我介绍？
```
git config --global user.name "huanghu996"
git config --global user.email “562904586@qq.com"
```
我们向git自我介绍之后，还要向github打招呼呀。

因为这年头骗子多，github只向可以信任的人打招呼。

## SSH KEY让github相信你
git命令行中运行如下命令在.ssh文件夹中生成ssh key
```
ssh-keygen -t rsa -C "562904586@qq.com"
```

最后在.ssh下会生成id_rsa和id_rsa.pub两个文件。

其中。pub文件是可以公开查看的，id_rsa要保密呀。

ssh key就像是一个令牌，有了它就可以畅通无阻的访问你在github上的库啦

### 将令牌（SSH KEY）的模样告诉github
Settings --》 SSH and GPG keys --》 填写好title（就是起个名字）--》将id_rsa.pub内容全部粘贴到Key中 --》 点击 Add SSH key

### 验证SSH key 有没有绑定成功
在shell里面输入
```
ssh -T git@github.com
```
就可以知道啦

## 如何向github自我介绍
在该目录下（.ssh）创建config文件
config文件（配置文件）这样写
```
Host github.com
User huanghu996
Hostname ssh.github.com
PreferredAuthentications publickey
IdentityFile ~/.ssh/id_rsa
Port 443
```

我们使用github的远程仓库，上传跟下载必不可少。
## 我们如何将远程仓库下载下来？
```
git clone git@github.com:huanghu996/.git
```
叫一声git，跟他说我们要clone，克隆git@github.com中的huanghu996用户的xxx.git仓库

## 创建分支
在电脑中我们可以建立许多文件夹，同样在项目中也可以建很多的分枝
通过一下代码我们可以查看当前已经有的分支
```
git branch
```
建立新分支
```
git checkout -b master1
```
它一下命令的简写
```
$ git branch master1
$ git checkout master1  //用来切换到分支master1
```
## 修改了文件，怎么更新github上的文件
我们先将文件放入暂存区（就是一个更新的队列）
```
git add . //这是将所有文件放入队列
```

因为上传github的文件都必须要评论，所以我们需要一下代码来添加评论
```
git commit -m "update "
```
### 下面需要的就是芜湖起飞
```
git push
```

# 大功告成！

## 学习Git中的脑残案例
1. 文件名打错/(ㄒoㄒ)/~~
1. 没有加入暂存区，push无论多少次都原地踏步。

# markdown

# 我是老大
## 我是老二
### 我是老三
#### 我是老四
##### 我是老五
###### 我是老六

段落  
段落

段落

*我是斜体*
**我是粗体**
***我是粗斜体***

-----------------------------------

~~我没了~~

<u>我有底线</u>

我是小姐姐[^查看真相]
[^查看真相]:真的是小姐姐

* 我是子标题
1. 我是子标题的儿子
* 我是第二个子标题

>我右移了一格
>>我右移了两格
>>>我右移了三格

`我是代码片`

```
我是代码块
```

在线发牌，加我vx [点我查看](/骗你的.com)

<img src="https://www.baidu.com/img/flexible/logo/pc/result.png"/>

|  时间   |  课程  |
|  :----  | :----:|
| 上午    | 高数   |
| 下午    | 大物   |

## 加入程序部想学的东西
1. UI设计啦，本人是审美黑洞
2. 向python大佬请教
3. 当然啦，如果能进一个项目组，我会很开心的

看到这里啦，谢谢学长学姐！
以后还要向你们多多学习，请教的！







