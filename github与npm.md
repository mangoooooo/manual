#一、通过npm安装github上的包  <big>
1.  进入项目文件夹： （这里以宿主机为例，虚拟机也差不多 ）  
	a)   运行cmd，进入相应盘，输入cd workspace/www/helloworld/hwtest  
2.  假如我要安装这个包：[https://github.com/expressjs/express](https://github.com/expressjs/express)  
	c)  获得这个包的地址：[https://github.com/expressjs/express.git](https://github.com/expressjs/express.git)  
	d)  命令行输入：npm install [https://github.com/expressjs/express.git](https://github.com/expressjs/express.git) 安装成功，效果如图：1-1　　
![图１－１](https://ooo.0o0.ooo/2016/10/31/581714afb8596.png)
3.  观察此刻的项目目录，会发现多了一些东西，如图1-2  
![图1-2](https://ooo.0o0.ooo/2016/10/31/581714afc2dbd.png)   
4.  关于使用，直接使用require就好，如：var express = require('express')
5.  注意，如果直接运行html页面可能会出现“require is not defined”这样的报错，那是因为nodejs 是在服务器端运行的，不能直接用在HTML上。</big>
	
#二、将github上的包发布到私有npm上  
1.  npm set registry http://192.168.100.230:4873    // 设置镜像，指向私有npm的地址
2.  npm config list     //  显示配置
3.  npm login
4.  进入到有package.json 的文件夹下
5.  npm publish，效果如图1-3