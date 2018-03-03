# JavaWeb 电商计划 v2.0

[![forthebadge](https://forthebadge.com/images/badges/made-with-java.svg)](https://forthebadge.com)&emsp;[![forthebadge](https://forthebadge.com/images/badges/powered-by-responsibility.svg)](https://forthebadge.com)&emsp;[![forthebadge](https://forthebadge.com/images/badges/uses-git.svg)](https://forthebadge.com)&emsp;[![forthebadge](https://forthebadge.com/images/badges/uses-js.svg)](https://forthebadge.com)

> 02/24/18 2.0开工，覆盖Tomcat集群+Nginx负载均衡+Redis分布式

![section2](http://oxgw3nd2b.bkt.clouddn.com/section2.jpg)

> 02/24/18 按照阿里巴巴Java代码规约插件规范代码，一期后端杀青

> 02/22/18 更新：Code Review & 添加“纯小白”风格注释中，勿黑

JavaWeb 初学项目，参考慕课网：https://coding.imooc.com/class/96.html
> 上线地址（备案中……🤣）：http://shuwuai.tech

### 开发环境
* 操作系统：macOS 10.13.3
* IDE：IntelliJ IDEA 2017.3.4
* JDK：JDK 1.8
* Web容器：Tomcat 9.0.2
* 数据库：Mysql 5.7.20 Community Server
* 依赖管理工具：Maven 3.5.2
* [Mybatis-PageHelper](https://github.com/pagehelper/Mybatis-PageHelper)
* [MyBatis Generator](http://www.mybatis.org/generator/index.html)
* [Mybatis plugin](https://www.codesmagic.com/mybatisplugin)
* 前后端接口测试  [Restlet Client - REST API Testing](https://restlet.com/modules/client/) 或  [Postman](https://www.getpostman.com/)

![Restlet Client](http://oxgw3nd2b.bkt.clouddn.com/2018-02-21_19-34-18副本.png)

* [支付宝 SDK](https://openhome.alipay.com/platform/home.htm)
* 其他依赖参见 `pom.xml`


### 个人推荐工具：🍻
* Code：Dash, Sublime Text 3
* 插件：AceJump, Material UI, Lombok, JRebel, Translation
* 码字：MWeb, Quiver, iText
* VCS：SourceTree
* 终端：iTerm 2, tmux, FinderGo, space-vim
* 数据库：mycli, Sequel Pro, Medis
* 网络：Charles, Gas Mask
* JVM：VisualVM
* Linux：Transmit, VMware Fusion
* 效率：Karabiner-Elements

## 后端部分一期核心
* SpringMVC + MyBatis
* 前后端分离
* 高复用服务响应对象的设计思想及抽象分装，ServerResponse<T> 对象承载，类比 `ModelAndView`

![ServerResponse](http://oxgw3nd2b.bkt.clouddn.com/ServerResponse.png)

## 模块构成
* 用户（登入登出、鉴权、注册、重置密码、获取/更新用户信息）
* 商品分类（详情页、商品列表分页）
* 购物车（商品总价计算、价格运算丢失精度问题）
* 订单（订单号生成规则、安全漏洞解决）
* 发货（SpringMVC 对象绑定、MyBatis 自动主键生成）
* 支付（支付宝对接、二维码沙箱测试）
* 线上部署（JDK/Maven/Tomcat/Nginx/vsftpd/Git、自动化发布）
* 接口测试  

**v1.0 / 部分2.0 测试用接口：[By Restlet_Client](https://github.com/shuwuai/tmall/wiki/%E6%8E%A5%E5%8F%A3%E6%B5%8B%E8%AF%95-By-Restlet_Client)**

![tmall](http://oxgw3nd2b.bkt.clouddn.com/tmall.png)

> 03/04/18 梳理用户模块逻辑

```
Request
Content-Type: 
application/x-www-form-urlencoded
Response 
Content-Type: 
application/json;charset=UTF-8
```


