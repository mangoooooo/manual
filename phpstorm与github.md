#一、前言
<big>
根据实际情况，利用phpstorm操作github最基本的目的无非两种：  

1.  从github上clone别人的代码，然后使用修改，再提交到github上pull request  
2.  把自己的项目，放到github上  

文章开始前，假设你已经：  

1.  安装好了git  
2.  有了github账号  
3.  安装好了phpstorm  
 

下面让我们正式开始。  
</big>
#二、从github上clone项目 
<big>
1.  第一步肯定是要在github上fork你需要的项目啦，这样你才有权限提交修改   
2.  phpstorm工具栏：VCS -> check from version control -> github，如图1-1：
![图1-1](https://ooo.0o0.ooo/2016/10/31/5816c053c064f.png)  
3.  第一次操作会弹出github登录框 ，随后还会弹出输入master密码的对话框，请记下来  
4.  弹出 clone Repository 对话框：  
　　a) git Repository url: 就是github上对应项目下，点击“Clone or download”弹出的地址啦  
　　b) parent directory: 你想把clone的文件放在哪  
　　c) directory name: 按你喜欢  
　　具体，如图1-2所示：  
![图1-2](https://ooo.0o0.ooo/2016/10/31/5816c3c89952b.png)  
5.  打开项目文件，可以看到项目已经checkout下来啦，如图1-3：  
![图1-3](https://ooo.0o0.ooo/2016/10/31/5816c4096a08e.png)  
6.  打开文件的时候，可能会弹出 add file to git 的对话框，我很懒，直接yes，也可以仔细看对话框的内容按需添加  
</big>
#三、修改clone下来的文件以及提交  
<big>前面我已经从github上clone了项目，现在如果我想修改某个文件或者添加新的文件，该如何操作呢？</big>  
##1.提交修改的文件
<big>
　　1.  假如我想修改 README.md 这个文件，会发现文件变色了！这代表这你对文件进行了修改，如图1-4：  
　　![图1-4](https://ooo.0o0.ooo/2016/10/31/5816c82639a96.png)  
　　2.  选择你想要提交的文件 -> 右键 -> git -> commit file , 如图1-5：  
　　![图1-5](https://ooo.0o0.ooo/2016/10/31/5816c85880f0b.png)  
　　3.  弹出commit changes对话框：  
　　　　a)  选择你要提交的文件  
　　　　b)  双击文件还可以看到你做了哪些修改   
　　　　c)  commit message : 一定要填！！对自己负责，对他人负责！尽可能的描述自己修改了什么 ！！！   
　　　　d)  选择commit and push ： 如果只选择commit的话，是之提交到本地的git，所以还要push；  
　　　　e)  你也可以先commit，再选择文件 -> 右键 -> git -> repository -> push , 这里我就直接 commit and push 啦，如图1-6：  
> ![图1-6](https://ooo.0o0.ooo/2016/10/31/5816c88cecbf2.png)  
　　4.  弹出push commits 对话框 ， 选择你要push的文件，如图1-7，为什么会有两个呢？那是因为有一次我点击的commit而没有commit and push，所以你大概知  道push的是你commit过的文件了吧？  
　　![图1-7](https://ooo.0o0.ooo/2016/10/31/5816c8b72dd30.png)  
　　5.  现在到github上刷新看看，是不是看到我修改的东西了？如图1-8：  
　　![图1-8](https://ooo.0o0.ooo/2016/10/31/5816c8f27e262.png)  
　　6.  剩下的就是github上的操作了，把你修改的东西pull request，具体的步骤我就简单描述一下：  
　　　　a) 点击图1-8中的new pull request  
　　　　b) 点击create pull requset，填写相应的描述之后，就create pull requset吧，等待matser的回复  
</big>
##2.在clone下来的项目中添加文件  
<big>
　　1.  加入我新增了一个文件叫test.txt，弹出add file to git对话框，这时候当然选择yes啦，如图1-9，文件是绿色的：  
![图1-9](https://ooo.0o0.ooo/2016/10/31/5816dd46858d8.png)  
　　2.  选中文件 -> 右键 -> git -> add， 对于新增的文件，需要先add再commit  
　　3.  选中文件 -> 右键 -> git -> commit  
　　4.  接下来的操作就跟上面第三点及之后一样啦，让我们来看看效果，如图1-10：  
![图1-10](https://ooo.0o0.ooo/2016/10/31/5816dd615a6d7.png)   
</big>
#四、把项目放置github上  
<big>假如我有项目jltTest，那如何把我的项目分享到我的github上呢？  
1.  打开项目jltTest，phpstorm工具栏：VCS -> import into version control -> share project on github，如图1-11  
![图1-11](https://ooo.0o0.ooo/2016/10/31/5816dda57b504.png)  
2.  弹出 share project on github 对话框，如图1-12  
![图1-12](https://ooo.0o0.ooo/2016/10/31/5816ddbf80f23.png)  
3.  选择你要share的文件，如图1-13  
![图1-13](https://ooo.0o0.ooo/2016/10/31/5816dddc65191.png)   
4.  第一次的话，会弹出输入master密码的对话框  
5.  分享成功，去github上看看，如图1-14  
![图1-14](https://ooo.0o0.ooo/2016/10/31/5816de0020e8e.png)</big>