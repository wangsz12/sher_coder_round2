#**程序部二面任务提交**

##1.git学习
    我学习了解git以及github的过程是从一次代码提交开始的。
    为了熟悉git以及GitHub的操作，我选择将自己国庆期间完成的vue.js主题下的demo作品代码提交到自己的代码库。
    
    第一次提交代码步骤：
    1.首先，注册GitHub账号，安装git客户端到自己的电脑。
    
    2.绑定用户——打开客户端，执行指令：git config -- （1）global user.name "填入GitHub账号" 
                                                 （2）git config --global user.email"填入GitHub相对应的邮箱"
    
    3.为GitHub账户设置SSH key：（1）在git客户端执行指令：ssh-keygen -t rsa -C "你的邮箱" 
                              （2）在git客户端执行指令：clip < ~/.ssh/id_rsa.pub（复制ssh key，便于后续创建）
                              （3）打开GitHub网页，进入setting找到ssh key并新建ssh key实例
                              （4）在git客户端执行指令：ssh -T git@github.com测试连接是否成功
    4.进入本地要提交项目文件的的所在位置打开Git Bash。
    
    5.依次在git客户端执行指令：（1）git init
                             （2）git add .
                             （3）git commit -m "提交描述"
                             （4）git remote add origin + 仓库地址
                             （5）git push -u origin master
    
    6.进入GitHub网页检查自己提交的代码
    
##2.学习Markdown
    Markdown是一种纯文本格式的标记语言。通过简单的标记语法，它可以使普通文本内容具有一定的格式。 因为是纯文本，所以只要支持Markdown的地方都能获得一样的编辑效果。Markdown编辑格式操作简单明了，只需要学习相关博客就可以熟练掌握，这里附上我所学习的其他人的博客地址：https://www.jianshu.com/p/191d1e21f7ed/
    
##3.Markdown实践

# 一级标题
## 二级标题
### 三级标题

**字体加粗**

*斜体*

***斜体加粗***

~~删除线~~

>引用的内容

分割线
---

[超链接](https://www.baidu.com/)

表格
表头|表头|表头
---|:--:|---:
内容|内容|内容
内容|内容|内容

(```)
    public static void main(String[]args){
         System.out.printf("代码块");
      }
(```)

