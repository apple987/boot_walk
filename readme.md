﻿工作业余时间，结合项目使用技术点，整合到SpringBoot中，目前升级到2.0.2版本,(码云提供有Mycat版本)，您的宝贵意见，是我们进步的动力。<br>
 <br> 
**具有如下特点**   
> * 友好的代码结构及注释，便于阅读及二次开发 。<br>
> * 前端页面采用freemarker,模板化引擎设计,页面采用bootstrap-table灵活强大的表格插件。<br>
> * 前端采用vkbeautify格式化JSON,XML,CSS,SQL显示。<br>
> * 后端配置swagger在线文档，方便编写API接口文档。 <br>
> * 引入druib,fastjson,cors,xss,redis-cluster配置。<br>
> * 引入API模板，根据token作为登录令牌，极大的方便了APP接口开发。<br>
> * 引入Hibernate Validator校验框架，轻松实现后端校验。<br>
> * 配置全局异常处理，通用日志打印,pagehelper分页。<br>
> * 配置redisson集群模式,使用分布式锁，保证并发的数据一致性。<br>
> * 配置全局errorPage和welcomeFile完善全局异常处理，优化异常处理代码。<br>
> * 配置devtools热部署，针对page目录下的css,js,html页面资源修改之后，项目不需要重新启动。<br>
> * 引入druib,javaMelody监控系统各项指标，分析系统瓶颈。<br>
> * 配置elastic-job定时器，强悍的分布式定时任务配置。<br>
> * 配置fileupload(默认配置最大100MB)，下载文件，生成二维码，二维码打印，mail发邮件等功能。<br>
> * 配置https安全协议，提高系统安全性,配置log4j日志，系统出现异常自动发送邮件。<br>
> * 配置poi和csv简单导出excel功能点,poi目前是多sheet智能导出。<br>
> * 配套代码生成工具，快速生成前后端代码，极大的提高开发效率。<br>
 <br> 
**项目结构** <br>
```
boot-walk<br>
├─doc  项目SQL语句<br>
│ <br>
├─common 公共配置<br>
│ <br>
├─framework 框架配置<br>
│ <br>
├─modules 功能模块<br>
│  ├─app API接口模块(APP调用)<br>
│  ├─controller 系统模块<br>
│  ├─mapper  mybatis的sql文件<br>
│  ├─model   数据库实体类<br>
│  └─service 业务逻辑层<br>
│ <br>
├─StartUpApplication 项目启动类<br>
│  <br>
├──resources <br>
│  ├─page 页面资源(static,view)<br>
│  ├─application.properties 配置文件<br>
│  ├─banner.txt  自定义启动图标<br>
│  ├─mybatis_config.xml mybatis配置项<br>
│  └─secure.jks  ssl安全证书<br>
```
<br> 
<br> 
 **环境配置:**<br>
- 1.项目依赖,redis-cluster集群,zookeeper,activeMq,solr工具,目前工具运行环境(win7 x64)。<br>
- 2.doc目录里面有初始化sql，运行项目前，请先创建mysql。<br>
- 3.工具地址:https://pan.baidu.com/s/1Bm7udGJc40xEENFgnJjsIw
<br> 
<br> 	 
 **启动说明:**<br>
- 1.创建mysql数据库isec实例,运行doc目录里面的sql文件。<br>
- 2.启动redis集群(127.0.0.1:6379~6384，密码:qdone)。<br>
- 3.启动activeMq(默认单机版)。<br>
- 4.启动solr(默认单机版)。<br>
- 5.启动zookeeper(默认单机版本2181)。<br>
- 6.运行StartUpApplication启动项目，浏览器访问http://localhost。<br>
 <br> 	
 **用户反馈：**<br>
- Git仓库： https://github.com/apple987/boot_walk <br>
- 码云仓库： https://gitee.com/bootstrap2table/boot_master<br>
- Mycat版本: https://gitee.com/bootstrap2table/boot_master/tree/feature/mycat<br>
- 代码生成： https://github.com/apple987/AutoCode<br>
- 邮箱地址:  m15171479289@163.com <br>

### 效果图
![boot-start](https://github.com/apple987/static/raw/master/boot/image/start.png "项目启动")<br>	
![boot-ssl](https://github.com/apple987/static/raw/master/boot/image/ssl.png "初始化")<br>
![boot-index](https://github.com/apple987/static/raw/master/boot/image/index.png "欢迎页")<br>
![boot-swagger](https://github.com/apple987/static/raw/master/boot/image/swagger.png "swagger在线文档")<br>
![boot-applogin](https://github.com/apple987/static/raw/master/boot/image/appLogin.jpg "app登陆接口")<br>
![boot-appGetUser](https://github.com/apple987/static/raw/master/boot/image/appGetUser.jpg "app获得登陆信息接口")<br>
![boot-emailError](https://github.com/apple987/static/raw/master/boot/image/emailError.jpg "邮件发送异常")<br>
![boot-runmq](https://github.com/apple987/static/raw/master/boot/image/runmq.jpg "发送MQ消息")<br>
![boot-mq](https://github.com/apple987/static/raw/master/boot/image/mq.jpg "MQ队列和订阅")<br>
![boot-selectStaff](https://github.com/apple987/static/raw/master/boot/image/selectStaff.jpg "职员信息列表")<br>
![boot-insertStaff](https://github.com/apple987/static/raw/master/boot/image/insertStaff.jpg "添加职员信息")<br>
![boot-insertError](https://github.com/apple987/static/raw/master/boot/image/insertStaffError.jpg "validate验证信息")<br>
![boot-durid](https://github.com/apple987/static/raw/master/boot/image/druid.png "durid监控")<br>
![boot-javaMelody](https://github.com/apple987/static/raw/master/boot/image/javaMelody.png "javaMelody监控")<br>	
![boot-qrcode](https://github.com/apple987/static/raw/master/boot/image/qrcode.png "生成二维码")<br>
![boot-print](https://github.com/apple987/static/raw/master/boot/image/print.png "打印二维码")<br>
![boot-solr](https://github.com/apple987/static/raw/master/boot/image/solr.png "solr导入数据")<br>
![boot-upload](https://github.com/apple987/static/raw/master/boot/image/upload.jpg "文本上传")<br>
![boot-uploadError](https://github.com/apple987/static/raw/master/boot/image/uploadError.jpg "文件上传异常")<br>
		
		

        
