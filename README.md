# 在线签字/远程签字/实名签字/密码签/电子签章/电子签字
## 平台介绍
本平台分为PC和App两端，pc端分为用户端以及管理员端，根据角色来区分；App支持普通用户使用。管理员可设置签字套餐内容，按次和时间来算。普通用户登陆后，先上传所需签字的文件，之后选择签字位置，一件发送至需签名的用户，通过短信或者app推送的方式通知到相关用户；收到签字消息通知后，点击短信/App推送的消息，跳转至预览界面，可点击签字进行手动签，如果之前签过，那么直接选择历史签名即可。签完之后，则通知到发起者，双方都可下载签完字的文档。签名有多种方式供用户选择，分别为：密码签、实名签、面对面签字等。
## 联系方式
手机：18612878499（wx）      李逍
## 技术选型

### 1. 环境

* Java SDK 1.8
* Apache Maven 3.6+
* 支持Docker、k8s等
### 2. 主框架

* Spring Boot 2.2
* Spring Websocket
* Apache Shiro 1.6
* Flowable
* Webpack
* Jwt
* Swagger
### 3.持久层

* Apache Mybatis 3.5
* Alibaba Druid 1.1
* Hibernate Validation 6.0（服务端验证）
* Sharding JDBC 4.0（读写分离、分库分表）
### 4.视图层

* Spring MVC 5.2
* Beel 3.1（视图模板引擎、替换JSP）
* CSS框架：
    * Bootstrap 3.3
    * AdminLTE 2.4
* JS框架及组件
    * Jquery 1.12
    * layer 3.1
    * zTree 3.5
    * jqGrid 4.7
    * jquery-validation
    * wdScrollTab
    * webuploader
    * uediter
    * toastr
###  5.工具组件

* Logback 1.2
* Apache Commons
* 对象序列化：FST 2.57
* JSON序列化：Jackson 2.10
* Office工具：POI 4.1
* 分布式任务调度：Quartz 2.3
* 全文检索引擎：ElasticSearch、Lucene
* 支付宝/微信在线支付
* 阿里云/极光短信
### 6.存储

* 数据库：mysql
* 缓存：Redis/ehcache
## 主要功能
### 1、PC端

* 签字次数提醒
    * 展示了用户剩余的签字次数，剩余量达到限定额后会自动提醒充值
* 签字列表
    * 展示了用户发起、参与的签字文件，可查看详情，多条件搜索，以及下载文档
* 发起签字
    * 首先先上传所需签字的文档，添加所要签字人的姓名及联系方式，然后选择签字人的签字位置，确定位置后，到达第三步，可复制生成的链接发送给需要签字的用户，或者直接通过短信的方式来通知到对方
* 我的签名
    * 保存了我的的历史签字，以便有签字需要时，快速签名
* 支付订单
    * 此功能展示了购买签字套餐所产生的订单
* 系统设置（管理员功能）
    * 套餐设置
    * 使用记录
    * 用户基础信息
    * 微信/支付宝/推送配置
    * App轮播图设置
    * 小程序设置
    * 初始套餐设置
### 2、APP端

* 注册、登录
    * 通过手机号+验证码/密码的方式注册/登录
* 首次注册有相应套餐赠送
* 发起签字--》选择签字人--》确认签字位置--》通知相关人员--》收到通知，打开链接--》查看文件，选择签字/历史签名，进行签字--》签字完成后--》通知发起人
* 在线微信支付购买套餐
* 可进行实名认证，使用实名签、密码签等功能
## 平台截图
### 1、PC
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/33/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-1.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/33/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-2.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/33/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-3.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/33/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-4.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/33/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-5.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/33/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-6.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/33/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-7.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/33/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-8.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/33/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-9.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/33/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-10.png)
### 2、APP
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/3%20(1)/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-1.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/3%20(1)/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-2.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/3%20(1)/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-3.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/3%20(1)/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-4.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/3%20(1)/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-5.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/3%20(1)/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-6.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/3%20(1)/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-7.png)
![Image text](https://raw.githubusercontent.com/fengkuangdongwuyuan/qz/main/image/3%20(1)/%E7%A8%BF%E5%AE%9A%E8%AE%BE%E8%AE%A1-8.png)
