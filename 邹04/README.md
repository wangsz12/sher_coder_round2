# 学习markdown的经历   
   - 学习markdown的第一天，由于没有仔细阅读任务一，导致我胡乱的学习。比如：通过看一些对话的源代码来学习，导  致学习效率极其低下。不过这也是件好事情，胡乱的学习使我接触到了很多碎片化的东西。  
>   - 学习markdown的第二天，我使用了菜鸟教程，使我在今天的学习中突飞猛进，学会了超多东西：  
>>   ### 1. 比如“#”的使用   
>>      #hello，world
>>   ### 2. 一级二级标题   
>>      # ## ### #### ##### ######  
>>   ### 3.*字* **体** ***的使用***
>>   ### 4.分隔线的使用  
>>   ***
>>   ### 5. ~~删除线的用法~~
>>   ### 6.列表   
>>   * 第一项   1.第一项
>>   * 第二项  
>>   ### 7.列表
>>   ### 8.代码   
```python
import turtle as t

def nose(x,y):#鼻子
    t.pu()
    t.goto(x,y)
    t.pd()
    t.seth(-30)
    t.begin_fill()
    a=0.4
    for i in range(120):
        if 0<=i<30 or 60<=i<90:
            a=a+0.08
            t.lt(3) #向左转3度
            t.fd(a) #向前走a的步长
        else:
            a=a-0.08
            t.lt(3)
            t.fd(a)
    t.end_fill()

    t.pu()
    t.seth(90)
    t.fd(25)
    t.seth(0)
    t.fd(10)
    t.pd()
    t.pencolor(255,155,192)
    t.seth(10)
    t.begin_fill()
    t.circle(5)
    t.color(160,82,45)
    t.end_fill()

    t.pu()
    t.seth(0)
    t.fd(20)
    t.pd()
    t.pencolor(255,155,192)
    t.seth(10)
    t.begin_fill()
    t.circle(5)
    t.color(160,82,45)
    t.end_fill()

def head(x,y):#头
    t.color((255,155,192),"pink")
    t.pu()
    t.goto(x,y)
    t.seth(0)
    t.pd()
    t.begin_fill()
    t.seth(180)
    t.circle(300,-30)
    t.circle(100,-60)
    t.circle(80,-100)
    t.circle(150,-20)
    t.circle(60,-95)
    t.seth(161)
    t.circle(-300,15)
    t.pu()
    t.goto(-100,100)
    t.pd()
    t.seth(-30)
    a=0.4
    for i in range(60):
        if 0<=i<30 or 60<=i<90:
            a=a+0.08
            t.lt(3) #向左转3度
            t.fd(a) #向前走a的步长
        else:
            a=a-0.08
            t.lt(3)
            t.fd(a)
            t.end_fill()

def ears(x,y): #耳朵
    t.color((255,155,192),"pink")
    t.pu()
    t.goto(x,y)
    t.pd()
    t.begin_fill()
    t.seth(100)
    t.circle(-50,50)
    t.circle(-10,120)
    t.circle(-50,54)
    t.end_fill()

    t.pu()
    t.seth(90)
    t.fd(-12)
    t.seth(0)
    t.fd(30)
    t.pd()
    t.begin_fill()
    t.seth(100)
    t.circle(-50,50)
    t.circle(-10,120)
    t.circle(-50,56)
    t.end_fill()

def eyes(x,y):#眼睛
    t.color((255,155,192),"white")
    t.pu()
    t.seth(90)
    t.fd(-20)
    t.seth(0)
    t.fd(-95)
    t.pd()
    t.begin_fill()
    t.circle(15)
    t.end_fill()

    t.color("black")
    t.pu()
    t.seth(90)
    t.fd(12)
    t.seth(0)
    t.fd(-3)
    t.pd()
    t.begin_fill()
    t.circle(3)
    t.end_fill()

    t.color((255,155,192),"white")
    t.pu()
    t.seth(90)
    t.fd(-25)
    t.seth(0)
    t.fd(40)
    t.pd()
    t.begin_fill()
    t.circle(15)
    t.end_fill()

    t.color("black")
    t.pu()
    t.seth(90)
    t.fd(12)
    t.seth(0)
    t.fd(-3)
    t.pd()
    t.begin_fill()
    t.circle(3)
    t.end_fill()

def cheek(x,y):#腮
    t.color((255,155,192))
    t.pu()
    t.goto(x,y)
    t.pd()
    t.seth(0)
    t.begin_fill()
    t.circle(30)
    t.end_fill()

def mouth(x,y): #嘴
    t.color(239,69,19)
    t.pu()
    t.goto(x,y)
    t. pd()
    t.seth(-80)
    t.circle(30,40)
    t.circle(40,80)

def body(x,y):#身体
    t.color("red",(255,99,71))
    t.pu()
    t.goto(x,y)
    t.pd()
    t.begin_fill()
    t.seth(-130)
    t.circle(100,10)
    t.circle(300,30)
    t.seth(0)
    t.fd(230)
    t.seth(90)
    t.circle(300,30)
    t.circle(100,3)
    t.color((255,155,192),(255,100,100))
    t.seth(-135)
    t.circle(-80,63)
    t.circle(-150,24)
    t.end_fill()

def hands(x,y):#手
    t.color((255,155,192))
    t.pu()
    t.goto(x,y)
    t.pd()
    t.seth(-160)
    t.circle(300,15)
    t.pu()
    t.seth(90)
    t.fd(15)
    t.seth(0)
    t.fd(0)
    t.pd()
    t.seth(-10)
    t.circle(-20,90)

    t.pu()
    t.seth(90)
    t.fd(30)
    t.seth(0)
    t.fd(237)
    t.pd()
    t.seth(-20)
    t.circle(-300,15)
    t.pu()
    t.seth(90)
    t.fd(20)
    t.seth(0)
    t.fd(0)
    t.pd()
    t.seth(-170)
    t.circle(20,90)

def foot(x,y):#脚
    t.pensize(10)
    t.color((240,128,128))
    t.pu()
    t.goto(x,y)
    t.pd()
    t.seth(-90)
    t.fd(40)
    t.seth(-180)
    t.color("black")
    t.pensize(15)
    t.fd(20)

    t.pensize(10)
    t.color((240,128,128))
    t.pu()
    t.seth(90)
    t.fd(40)
    t.seth(0)
    t.fd(90)
    t.pd()
    t.seth(-90)
    t.fd(40)
    t.seth(-180)
    t.color("black")
    t.pensize(15)
    t.fd(20)

def tail(x,y):#尾巴
    t.pensize(4)
    t.color((255,155,192))
    t.pu()
    t.goto(x,y)
    t.pd()
    t.seth(0)
    t.circle(70,20)
    t.circle(10,330)
    t.circle(70,30)

def setting(): #参数设置
    t.pensize(4)
    t.hideturtle()
    t.colormode(255)
    t.color((255,155,192),"pink")
    t.speed(1000)



if __name__ == '__main__':
    setting() #画布、画笔设置
    nose(-100,100) #鼻子
    head(-69,167) #头
    ears(0,160) #耳朵
    eyes(0,140) #眼睛
    cheek(80,10) #腮
    mouth(-20,30) #嘴
    body(-32,-8) #身体
    hands(-56,-45) #手
    foot(2,-177) #脚
    tail(148,-155) #尾巴
    t.done() #结束  
 ```
    - 这是一个莽猪佩奇代码 
   在此感谢这段代码的主人 [peppa-pig](https://blog.csdn.net/sinat_36184075/article/details/80357696)  
    
   [小猪佩奇](https://image.baidu.com/search/detail?ct=503316480&z=0&ipn=d&word=%E5%B0%8F%E7%8C%AA%E4%BD%A9%E5%A5%87&step_word=&hs=0&pn=54&spn=0&di=208780&pi=0&rn=1&tn=baiduimagedetail&is=0%2C0&istype=0&ie=utf-8&oe=utf-8&in=&cl=2&lm=-1&st=undefined&cs=2926941908%2C3166064849&os=1565944035%2C242329279&simid=4103861248%2C574300300&adpicid=0&lpn=0&ln=1459&fr=&fmq=1601647157738_R&fm=&ic=undefined&s=undefined&hd=undefined&latest=undefined&copyright=undefined&se=&sme=&tab=0&width=undefined&height=undefined&face=undefined&ist=&jit=&cg=&bdtype=0&oriquery=&objurl=http%3A%2F%2Fwww.agri35.com%2FUploadFiles%2Fimg_0_1969236747_3922752013_26.jpg&fromurl=ippr_z2C%24qAzdH3FAzdH3Fooo_z%26e3Bw26tnc_z%26e3Bv54AzdH3FrtvAzdH3F%25Ec%25Ba%25bF%25E0%25bC%25AA%25E9%25BD%25Al%25Ec%25Ac%25b0%25E0%25l9%25lF%25Em%25Ba%25l9%25Em%25l0%25Bm%25Ec%25ba%25ll%25E0%25lA%25b9%25Em%25bn%25bc%25E9%25BE%25An%25Ec%25A9%25B9%25Ec%25bn%25bFAzdH3F&gsm=37&rpstart=0&rpnum=0&islist=&querylist=&force=undefined)  
   
>   - 学习markdown的第三天  
>>  ### 1.学习表格的制作  
>>  | 我学习的进度 | 
>>  | ---- |  
>>  | 0 |  
>>  | 0 |  
>   - ### 2.高级操作  
>>  <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>A</kbd> 截图  
>>  - ### 3.\*文本正常显示\*  
>>  - ### 4. 公式表示没学懂  
>>  - ### 5.[这是一个链接](www.4399.com)
***
***
***
## 进程序部~~的目的~~想学的东西
> 1. 人总是有目的性，当然，我的目的是好的，我进程序部便是想学Python，微信小程序的开发，界面设计，甚至是偷学一点公众号的运营（目前想学的有这些，以后会学习更多）。当然这个目的可以使我们双方受益，我会尽力学习，卖力为程序部工作
> 2. 暑假便开始想进升华工作室，权衡过后便是想进程序部
> 3. 未来职业规划是进入某东成为一名交通算法设计师，这与程序离不了干系
