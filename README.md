# 基于springboot2+vue2.X的校园招聘系统

系统源码可以完美运行，系统的视频非常详细，详细地讲解了系统的功能编写。

求个star，感谢！

**项目视频讲解地址**：https://www.bilibili.com/video/BV1FT4y1L7TA

## 1.系统简介

该系统基于springboot2，vue2.X等技术实现了校园招聘系统，为求职者与招聘人员提供了便捷的在线招聘信息平台。

### 1.1 系统环境配置

* 系统开发平台：JDK1.8+Windows7+Maven3.6.1

* 开发语言：JavaEE+vue

* 后台框架：Springboot

* 前端：Vue2.9.6

* 数据库:MySql5.7

* 开发环境: Intelij Idea

* 浏览器: Chrome或360浏览器

### 1.2 系统搭建步骤

前置条件：系统已经安装了Mysql5.7，Mysql工具(Navicat)，JDK1.8，Maven3.6.1，vue3.0以下开发环境，Intelij Idea，Chrome或360浏览器

* 导入数据库

* 编译前端代码vue：编译(cnpm install),试运行(npm serve)

* 导入后端代码springboot

* 启动springboot

### 1.3 首页

位于首页最上方的是导航栏，系统导航栏有：首页，招聘信息，求职者信息，友情链接，留言板，后台管理，登录

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/182903_15f2074b_7604956.png "屏幕截图.png")

导航栏下方是一个轮播图轮放图片，再往下是首页展示的招聘信息，求职者信息，新闻资讯等简略的内容，都可以点击查看更多来查看详细内容，该按钮对应导航栏的相应内容

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/183659_e8a39d38_7604956.png "屏幕截图.png")

首页的最下方是留言面板，需要登录才能留言

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/183741_a99d228a_7604956.png "屏幕截图.png")

### 1.4 招聘信息

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/183831_e8e53008_7604956.png "屏幕截图.png")

### 1.5 求职者信息

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/184037_60026e14_7604956.png "屏幕截图.png")

### 1.6 友情链接

可以和哪些网站进行互相链接访问

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/184103_6d515200_7604956.png "屏幕截图.png")

### 1.7 留言板

位于首页底部，登录的用户可以进行留言，管理员可以在后台查看留言。

### 1.8 后台管理

在个人中心点击我的后台或者直接在导航栏点击后台管理即可进入后台页面

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/204020_a21697f5_7604956.png "屏幕截图.png")

### 1.9 登录

登录分为用户登录和企业以及管理员登录

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/185136_e4944e14_7604956.png "屏幕截图.png")

管理员功能：用户管理，企业信息管理，岗位分类管理，学历信息管理，友情链接管理，系统管理，我的收藏管理，管理员管理，招聘信息管理等

用户功能：见个人中心

企业功能：招聘信息管理，应聘信息管理等

### 1.10 个人中心

登录之后导航栏会出现个人中心，点击可以查看个人信息，提供查看后台/退出登录/修改密码/修改个人信息等功能

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/184813_bcf76671_7604956.png "屏幕截图.png")

## 3. 导入后端代码并启动

启动IDEA，点击configure-settings

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/190753_47298c80_7604956.png "屏幕截图.png")

找到maven配置界面(Build，Execution，Deployment—Build tools—maven)，更改如下三个配置，改为自己电脑maven的位置即可

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/190817_ad5d67cc_7604956.png "屏幕截图.png")

点击ok，返回idea启动界面，点击open，找到项目位置，点击确定后等待项目下载依赖的包

点击pom.xml文件，查看文件是否有错误，如果有错误显示的是红色，如下错误，删除version行即可

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/191417_3f24f4aa_7604956.png "屏幕截图.png")

在pom.xml文件中点击鼠标右键-maven-reimport，强制自动重新加载

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/191545_857f7310_7604956.png "屏幕截图.png")

点击src-main-resources-application.yml，初始设置的端口号为8080，如果被占用则修改

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/191728_e065e991_7604956.png "屏幕截图.png")

确认数据库连接信息

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/191757_d40daba4_7604956.png "屏幕截图.png")

在src-main-java-com目录下找到SpringBootSchemaApplication.java，这是程序的启动类，点击鼠标右键，以debug方式启动程序

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/192030_16b37bd1_7604956.png "屏幕截图.png")

打开localhost:8080/springbootjlvpC/front/index.html访问前端页面，如果能看到页面，说明项目启动成功！

## 4. 框架介绍

### 4.1 pom.xml

相当于传统项目里面的jar包集合，使用maven导入项目，项目下的pom.xml是jar包的管理文件

### 4.2 项目层次

** controller**：调用service层

** dao**：包含数据库访问接口

** service**：包含接口和实现类

## 5. 后台vue架构

**启动后台**

定位到src/main/resources/admin.admin，右键点击admin.admin，选择show in explorer

切换到文件目录后，点击admin，进入admin文件夹内部

打开命令提示符窗口，定位到当前目录

执行**npm run serve

等待启动成功！

访问localhost:8081可以访问后台首页

8081端口在如下文件中指定：

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/172614_029dc073_7604956.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/172255_653d02a4_7604956.png "屏幕截图.png")

**注意事项**：确保已经执行安装，admin目录下有node_moudles文件夹

**main.js文件**

文件路径：src/main/resources/admin.admin/src/views/main.js

功能：整个vue项目的入口文件，引入了非常多的插件以供使用

从网页进入8081端口后会根据你是否登录进行相应的页面跳转，如果登录且登录没有过期会返回一个TOKEN给程序后台，返回上次关闭的页面，如果没有登录就直接进入登录页面

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/174722_6115b91e_7604956.png "屏幕截图.png")


## 6. 后台登录功能

**login.vue**

登录界面的背景图片相对路径的img文件夹下bg.jpg

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/175249_517cd476_7604956.png "屏幕截图.png")

rulesform定义了登录界面登录框的内容

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/175459_86c64f1c_7604956.png "屏幕截图.png")

账号的内容用到了v-model，即vue中的双向绑定，当账号的值在任何一个地方变化时会直接反馈回来

下面的代码对menu列表进行遍历，menu列表定义在页面启动之后进行加载，是一个长度为3的数组，可以使用json.com进行在线解析menu.js中的内容

el-radio为单项选择按钮，对登录身份进行选择

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/180124_ec378e22_7604956.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/180021_bb1af54d_7604956.png "屏幕截图.png")

注册用户与注册信息按钮中的@click意思是如果点击这两个选项的话会将相应的参数传到注册的函数register中

最下面是登录按钮，@click中绑定了login()函数，login函数执行逻辑可以参见视频

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/182138_25b76951_7604956.png "屏幕截图.png")

selectone需要传入一个wrapper参数，即条件构造抽象类，定义了T-SQL语法，可以看作是一个实体对象，帮我们简化sql语句

EntityWrapper可以将数据库表映射为一个实体类，这里映射的就是数据库中的user表

.eq有两个参数一个是列名一个是列的值，这一列等于这一个参数

返回值R是一个json数据，继承了hashmap，R的构造器中，若code等于0前端认为是一个正确数据，如果错误，code返回非0数据。

如果输入密码错误，返回R.error，如果输入密码正确，返回R.ok().put("token"，token)

generatiToken用来生成Token，它的参数包括从后台查询到的userid，username，users表名，角色值 

vue拿到了token之后，再登录之后就有权限向后台发送请求，在所有需要过滤的地方都会经行token验证，前端访问会把token放到header里面，用getHeader获取token

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/184222_903e432a_7604956.png "屏幕截图.png")

## 7. 后台首页功能

登录成功之后会进入index页面

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/185905_9a15b173_7604956.png "屏幕截图.png")

在进入之前会将token，role，sessionTable，admin信息放到storage缓存里面，对应数据库中的token表中的信息

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/185938_ad36d1bf_7604956.png "屏幕截图.png")

**index.vue**

index-header:后台首页上面的部分，这部分的功能在IndexHeader.vue中定义，包括管理员信息和退出登录功能

index-aside：后台首页左侧部分，这部分的功能在IndexAsideStatic中定义，提供个人中心，用户管理，企业信息管理等功能，点击按钮即可跳转到对应的页面

index-main：后台首页右侧部分

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/192536_4d9a4bce_7604956.png "屏幕截图.png")

## 8. 后台-个人中心

拿个人中心修改密码功能举例，在IndexAsideStatic中定义了一个@click="menuHandler("UpdatePassword")

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/193250_36f184cb_7604956.png "屏幕截图.png")

在route-static.js中查找修改密码的路由文件

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/193533_c4fd8e7d_7604956.png "屏幕截图.png")

对应views文件下的update-password

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/193607_28b8bf1a_7604956.png "屏幕截图.png")

查看views中的update-password文件，定义了修改密码页面的显示信息以及一些触发事件，包括检测密码是否为空，两次输入密码是否一致等

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/193707_470794b2_7604956.png "屏幕截图.png")

## 9. 后台-用户管理功能

显示用户信息，包括新增，删除用户，查看详情的功能

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/194216_a7dfd552_7604956.png "屏幕截图.png")

后台进入部分的代码，会进行一个遍历根据当前登录用户的权限得到backMenu

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/194440_265de458_7604956.png "屏幕截图.png")

在根据得到的backMenu进行遍历，再遍历得到内容的子项

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/194642_36f452b5_7604956.png "屏幕截图.png")

## 10. 后台编译vue

后台的代码是用vue和springboot前后端分离写的，vue的代码在写完成之后如果短时间内不需要做修改则可以进行编译，生成静态的html+js文件

定位到admin.admin文件夹目录下，打开命令提示符窗口，运行nmp build命令

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/195511_748c15da_7604956.png "屏幕截图.png")

编译完成后会多一个dist的文件夹，打开后里面会有一个html文件

后端访问页面的地址改变，变为

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/195708_f7c9477e_7604956.png "屏幕截图.png")

其余功能基本不变，为了使程序运行更快，可以删除admin.admin下的node_modules文件夹

## 11. 前台-轮播图功能介绍

查看index.html文件，下面的代码指向的是home.html文件，将这个页面包含到了index页面的下面，所以首页也会显示home页面的信息

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/200259_47936b97_7604956.png "屏幕截图.png")

section中定义的是轮播图的功能

![输入图片说明](https://images.gitee.com/uploads/images/2020/1219/200532_d361940d_7604956.png "屏幕截图.png")

## 12. 系统打包运行

点击IDEA右侧的maven，找到Lifecycle中的package，双击即可进行打包

打包成功后，找到打包的目录

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/193456_54927fa6_7604956.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/193522_b85a186c_7604956.png "屏幕截图.png")

**注意事项**：

删除以下文件，admin.admin中只留一个dist文件即可

![输入图片说明](https://images.gitee.com/uploads/images/2020/1218/193315_d7dfdc8f_7604956.png "屏幕截图.png")

运行jar包前要关闭idea中的程序，不然会有端口冲突


                                                **欢迎大家一起交流学习，共同进步。技术交流群，请加小孟微信：**

<div align=center><img width="150" height="150" src="https://images.gitee.com/uploads/images/2020/1219/203754_ef21dcd8_7604956.png"/></div>





