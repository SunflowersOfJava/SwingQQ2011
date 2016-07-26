【已有功能】
===========
1、服务端开启服务
2、客户端根据用户名和密码进行登录
3、简单的换肤(效果不是很好)
4、一对一文字聊天(很严重的bug)
5、截图功能
【数据库说明】
===========
数据库使用的是smallsql;

数据库使用：

把smallsql.jar放到和数据库(qqdb)同一级目录,  java -jar smallsql.jar.
在dos窗口下，输入 USE qqdb  回车两下
select * from userinfos  回车两下
select * from users 回车两下
select * from friend 回车两下

由于是随便玩玩的，表设计的很简单，现在才3张表。用户表users、用户信息表userinfos、好友表friend,表的字段可以参考user.hbm.xml、userinfo.hbm.xml和friend.hbm.xml。
使用hibernate对数据库进行访问;

【结构说明】
===========
项目文件夹说明:<br/>
<pre>
|--src 源代码<br/>
   |--org.fw 一些基本控件<br/>
   |--org.fw.cellrender 渲染<br/>
   |--org.fw.data JList等控件的使用到的数据<br/>
   |--org.fw.db.pojo hibernate用到的pojo类<br/>
   |--org.fw.event 自定义事件类<br/>
   |--org.fw.image 获取图片<br/>
   |--org.fw.manager RepaintManager<br/>
   |--org.fw.qq qq客户端相关类<br/>
   |--org.fw.qq.plugins.screencut 截图插件<br/>
   |--org.fw.qq.server qq服务端相关类<br/>
   |--org.fw.test 一些测试类<br/>
   |--org.fw.utils 一些帮助类<br/>
|--cfg 资源配置文件<br/>
|--info smallsql使用的一些截图<br/>
|--lib <br/>
|--qqdb 系统数据库<br/>
|--skin 用到的相关图片<br/>
</pre>
【原始数据】
===========
随便玩玩的，所以注册添加好友这些都没弄,要添加新的数据就用sql语句来添加吧。

测试账号:786074249,914001405,442714254,5201314 密码都是123456

【操作步骤】
===========
先运行org.fw.qq.server的QQServer类再运行org.fw.qq的Main类

【存在问题】：
===========
随便练练手的，所以没什么计划，就开始乱写了。想一点写一点，到后面发现想写好也变得很困难了。
界面的重绘存在很大的问题；
很多细节方面还存在很大的问题；
对于语音和视频聊天，只是简单的做了下尝试，代码基本上是网上拿来主义。
【应用截图】
===========
登录
![login](https://github.com/SunflowersOfJava/SwingQQ2011/tree/master/readme/login.png)
截屏
![cutscreen](https://github.com/SunflowersOfJava/SwingQQ2011/tree/master/readme/cutscreen.png)
好友列表
![friendlist](https://github.com/SunflowersOfJava/SwingQQ2011/tree/master/readme/friendlist.png)
日志
![logining](https://github.com/SunflowersOfJava/SwingQQ2011/tree/master/readme/logining.png)
皮肤设置
![skinset](https://github.com/SunflowersOfJava/SwingQQ2011/readme/skinset.png)
聊天
![skinset](https://github.com/SunflowersOfJava/SwingQQ2011/readme/talk.png)
视频聊天
![videotalk](https://github.com/SunflowersOfJava/SwingQQ2011/tree/master/readme/videotalk.png)
