# Github Copilot的申请以及在Pycharm的配置与使用详解

GitHub在联合OpenAI推出了一款"GitHub Copilot"工具,可以根据上下文自动写代码,下面这篇文章主要给大家介绍了关于Github Copilot的申请以及在Pycharm的配置与使用的相关资料,文中通过图文以及实例代码介绍的非常详细,需要的朋友可以参考下

## 前言

目前Github Copilot不是完全公开的，需要自己进入copilot官方网站进行申请，我申请下来是花了两天左右的时间。



## 1.简介

微软与OpenAI共同推出了一款AI编程工具GitHub Copilot。

GitHub Copilot基于 GitHub 及其他网站的源代码，可根据上文提示为程序员自动编写下文代码。

我使用下来它最实用的功能并不是说它的智能输入代码，而是它能够结合你实际业务代码的上下文进行预测你下一步的代码，会根据你的代码格式代码规范进行编写。

从个人的角度来讲，它带给我们的是更加便捷轻巧，当然，不能完全把它当作一个偷懒的工具，在一些灵活性逻辑比较复杂的一些功能上还需要我们自己验证，否则之后编译出错，你自己都找不到在哪里出问题。



## 2.copilot首页

https://copilot.github.com/

点击sign up 使用自己的github账户

![img](E:\GitHub\GPT\copilot\2022042610042128.jpg)



## 3.copilot的申请

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042129.png)

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042130.png)

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042131.png)



## 4.GitHub Copilot 官方使用文档

https://github.com/github/copilot-docs



## 5.PyChram下载地址

为什么会有这一步？

官方文档给出的说明：

- We have tested with the following JetBrains IDEs: IntelliJ and PyCharm versions 2021.2 and above.

意思是 经过他们的测试， JetBrains系列的 IntelliJ 和 PyCharm 这两款编译器需要使用2021.2及以上的版本

https://www.jetbrains.com/pycharm/download/other.html

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042132.png)



## 6.Pychram下载 GitHub Copilot

在pycharm中的Plugins中搜索GitHub Copilot点击Install进行下载（下载完别忘记了点击Apply哦）

![img](E:\GitHub\GPT\copilot\2022042610042133.jpg)



## 7.jetbrains系列官方教程

https://github.com/github/copilot-docs/blob/main/docs/jetbrains/gettingstarted.md#getting-started-with-github-copilot-in-jetbrains



## 8.申请通过之后的操作

等了两天，发邮件通知我通过了

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042134.png)

既然通过了，我们可以在Tools – > GitHub Copilot中进行登录自己的Github账号进行验证

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042135.png)

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042136.png)

**点击Join the Waitlist**

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042137.png)

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042138.png)



## 9.使用过程

如下为我的使用过程

写注释，然后回车就会发现它会给门智能建议代码，我们只需要按下Tab键，就会选择这个建议，然后会有新的建议代码出现，符合你的需求就继续按Tab键，比如我们按下四次Tab键后得到如下结果

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042139.gif)

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042140.gif)

![请添加图片描述](E:\GitHub\GPT\copilot\2022042610042141.gif)

除了以上的这些功能，你还可以在自己的业务代码里面尝试写一个新的方法，它会很智能的给出相关建议（需要自己确认一遍是否有误）

**Github Copilot自动生成的代码**

```
# 写一个函数，判断是否为回文数
# 回文数是指正序和倒序读都一样的数，例如12321，909
# 写一个函数，判断是否为回文数
# 回文数是指正序和倒序读都一样的数，例如12321，909
def is_huiwen(num):
    str_num = str(num)
    if str_num == str_num[::-1]:
        return True
    else:
        return False

# 冒泡排序
def maopao(list_num):
    for i in range(len(list_num)):
        for j in range(len(list_num)-i-1):
            if list_num[j] > list_num[j+1]:
                list_num[j],list_num[j+1] = list_num[j+1],list_num[j]
    return list_num

# 快速排序
def quick_sort(list_num):
    if len(list_num) <= 1:
        return list_num
    else:
        base = list_num[0]
        left = [x for x in list_num[1:] if x < base]
        right = [x for x in list_num[1:] if x >= base]
        return quick_sort(left) + [base] + quick_sort(right)

```



## 10.相关功能键：

- Tab选择提供的建议
- Esc拒绝提供的建议
- Alt+]查看下一个建议；Alt+[查看上一个建议。（macos把Alt键换成option键即可）
- Alt + \ 把提供的建议注释掉。（macos把Alt键换成option键即可）
- Alt+Enter显示当前所有的建议。（macos把Alt键换成option键即可）



## 11.退出Github Copilot

Tools – > GitHub Copilot – > Logout



## 总结

到此这篇关于Github Copilot的申请以及在Pycharm的配置与使用的文章就介绍到这了,更多相关Github Copilot在Pycharm的使用内容请搜索脚本之家以前的文章或继续浏览下面的相关文章希望大家以后多多支持脚本之家！

**您可能感兴趣的文章:**

- [浏览器不能正常访问Github的问题解决](https://www.jb51.net/article/253649.htm)
- [Github创建个人访问Tokens令牌](https://www.jb51.net/article/245727.htm)
- [JS一分钟在github+Jekyll的博客中添加访问量功能的实现](https://www.jb51.net/article/208844.htm)
- [提高github下载速度的方法可达到2MB/s(100%有效)](https://www.jb51.net/article/193185.htm)
- [配置Git并从GitHub上克隆项目](https://www.jb51.net/article/245732.htm)
- [github访问速度慢的问题完美解决](https://www.jb51.net/article/258536.htm)