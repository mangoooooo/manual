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
2.  phpstorm工具栏：VCS -> check from version control -> github  
3.  第一次操作会弹出github登录框 ，随后还会弹出输入master密码的对话框，请记下来  
4.  弹出 clone Repository 对话框：  
　　a) git Repository url: 就是github上对应项目下，点击“Clone or download”弹出的地址啦  
　　b) parent directory: 你想把clone的文件放在哪  
　　c) directory name: 按你喜欢      
</big>
#三、修改clone下来的文件以及提交  
<big>前面我已经从github上clone了项目，现在如果我想修改某个文件或者添加新的文件，该如何操作呢？</big>  
##1.提交修改的文件
<big>
　　1.  假如我想修改 README.md 这个文件，会发现文件变色了！这代表这你对文件进行了修改  
　　2.  选择你想要提交的文件 -> 右键 -> git -> commit file   
　　3.  弹出commit changes对话框：  
　　　　a)  选择你要提交的文件  
　　　　b)  双击文件还可以看到你做了哪些修改   
　　　　c)  commit message : 一定要填！！对自己负责，对他人负责！尽可能的描述自己修改了什么 ！！！   
　　　　d)  选择commit and push ： 如果只选择commit的话，是之提交到本地的git，所以还要push；  
　　　　e)  你也可以先commit，再选择文件 -> 右键 -> git -> repository -> push     
　　４.  现在到github上刷新看看，可以看到修改的东西了
</big>
##2.在clone下来的项目中添加文件  
<big>
　　1.  加入我新增了一个文件叫test.txt  
　　2.  选中文件 -> 右键 -> git -> add， 对于新增的文件，需要先add再commit  
　　3.  选中文件 -> 右键 -> git -> commit  
　　4.  接下来的操作就跟上面第三点及之后一样啦
</big>
#四、把项目放置github上  
<big>假如我有项目jltTest  
1.  打开项目jltTest，phpstorm工具栏：VCS -> import into version control -> share project on github  
2.  弹出 share project on github 对话框  
3.  选择你要share的文件   
4.  第一次的话，会弹出输入master密码的对话框  
5.  分享成功，去github上看看
</big>
