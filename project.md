#### **1.WiFi密码:** px51708610

#### **2.接口文档:** 
运行项目，访问[http://localhost:15111/doc.html](http://localhost:15111/doc.html)

#### **3.监控平台:**

|  说明   | 路径 |
| :---------: | :--: |
| 查看服务状态 |  http://localhost:8404/targets  |
| 查看alerts告警服务 |  http://localhost:8406/#/alerts  |
| Grafana可视化 |  http://localhost:8403/d/MQWgroiiz/mysql-jian-kong-mian-ban?orgId=1&refresh=1m  |

#### **4.项目地址:**

|   Git仓库  | Git仓库名 |  Git仓库地址 |
| :--------- | :--: | :-----------: |
| BMP-Vue |  前端vue项目  | http://zhaolihua@192.168.10.67:1010/r/BMP-Vue.git |
| BMP-Project   |  后端项目  | http://zhaolihua@192.168.10.67:1010/r/BMP-Project.git |
| 文档 |  文档  | http://zhaolihua@192.168.10.67:1010/r/文档.git |

#### **5.Git分支说明:**

|   Git分支  | 分支名称 |
| :---------: | :--: |
| master |  主分支(生产)  |
| dev   |  开发分支  | 
| release |  测试分支  | 
| uat |  预生产分支  | 

#### **6.开发工具:**

|  说明   | 工具 |
| :---------: | :--: |
| 前端 |  VsCode  |
| 后端   |  idea  | 
| 代码托管工具 |  Git  | 
| 项目打包部署 |  Jenkins  | 

#### **7.项目架构:**

**前端:** Node、Vue-Cli3

**后端:** 

|   说明  | 架构 |
| :---------: | :--: |
| JDK |  JDK8  |
| 数据库 |  MySQL 8.0.18  |
| 缓存 |  Redis、MongoDB  |
| 日志 |  Logback  |
| 持久层 |  Mybatis-Plus  |
| 工具类 |  Hutool、Guava  |
| 基础框架 |  SpringBoot、SpringCloud  |
| 全文搜索 |  ElstaticSearch、Kibana、Logstash  |
| 安全框架 |  Spring Security Oauth2  |
| 定时任务 |  Quartz  |
| 接口文档 |  Swagger-Ui、Knife4j  |
| 远程调用 |  Feign  |
| Excel导出 |  EasyExcel、EasyPoi  |
| 数据库文档 |  screw  |
| 分布式事务 |  TX-LCN  |
| 监控系统 |  SpringBoot-Admin  |
| 注册配置中心 |  Nacos  |
| 可视化平台 |  Prometheus、Grafana、AlertManager  |
| 其他插件 |  FastJson、Lombok  |

#### **8.服务模块:**

- **系统模块:**

| 服务名称  | 端口 |        描述       |
| :---------: | :--: | :-------------:|
| px-bmp-auth |  8101  |  微服务授权认证服务器 |
| px-bmp-gateway |  15111  |  微服务网关 |
| px-bmp-base |  8201  |  微服务子系统，基础数据模块 |
| px-bmp-user |  8301  |  微服务子系统，系统管理模块 |
| px-bmp-chain |  8401  |  微服务子系统，WMS模块 |
| px-bmp-erp |  8501  |  微服务子系统，ERP模块 |
| px-bmp-order |  8601  |  微服务子系统，OMS模块 |
| px-bmp-job |  8701  |  微服务子系统，任务调度模块 |
| px-bmp-monitor |  8801  |  微服务监控子系统 |
| px-bmp-generator |  8901  |  微服务子系统，代码生成器 |
| px-bmp-tx-manager |  8888  |  微服务分布式事务控制器 |


- **第三方模块:**

| 服务名称  | 端口 |        描述       |
| :---------: | :--: | :-------------:|
| Nacos |  8761  |  注册中心、配置中心 |
| MySQL |  3306  |  数据库 |
| Redis |  6379  |  K-V缓存数据库 |
| MongoDB |  27017  |  缓存数据库 |
| ElasticSearch |  9200  |  日志存储 |
| Kibana |  5601  |  日志展示 |
| Logstash |  9600  |  日志收集 |
| Minio |  9000  |  文件服务器 |
| Gitblit |  1010  |  Git服务器 |
| Jenkins |  8086  |  自动化部署 |
| Grafana |  8403  |  监控告警平台 |
| Prometheus |  8404  |  监控告警平台 |
| AlertManager |  8406  |  监控告警平台 |
| mysqld_exporter |  8409  |  监控MySQL |
| showdoc |  8888  |  接口管理平台 |
#### **9.奇门对接:**

###### **1.奇门申请**

1.在奇门仓储接入说明中[https://open.taobao.com/doc.htm?docId=106850&docType=1](https://open.taobao.com/doc.htm?docId=106850&docType=1),
选择适合你的业务场景，目前奇门申请的账号选择的业务场景是**非淘ERP**，点击申请。
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/1.png)

###### **2.创建应用**

2.然后根据自己的场景创建应用，申请通过之后，在**应用管理**，可以看到创建好的app_key和secert
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/2.png)
也可以通过该步骤创建应用:(入驻成为开发者——创建应用(获得appKey和secert及下载SDK)——开发测试——发布上线)
具体参考[https://open.taobao.com/doc.htm?docId=118395&docType=1&source=search](https://open.taobao.com/doc.htm?docId=118395&docType=1&source=search)

###### **3.SDK下载**

3.根据开发环境下载SDK
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/3.png)

###### **4.奇门API文档**

4.奇门仓储文档，点击文档中心或此链接，[https://open.taobao.com/api.htm?spm=a219a.7386653.0.0.d467669ayt8Fff&docId=24690&docType=2&source=search](https://open.taobao.com/api.htm?spm=a219a.7386653.0.0.d467669ayt8Fff&docId=24690&docType=2&source=search)

5.具体字段参考奇门白皮书

###### **5.接入奇门仓储**

6.点击控制台->选择奇门->点击场景列表，接入奇门仓储业务->点击我的场景，选择已上线的应用，选择业务角色,创建成功之后点击进入
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/4.png)
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/5.png)

###### **6.奇门API自测**

7.点击需要接入的API接口，进行自测，配置自测服务地址->编辑用例，填写接口名称和报文->点击自测按钮，返回200则表示自测成功
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/6.png)
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/7.png)
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/8.png)
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/9.png)

###### **7.奇门API联调**

8.配置与WMS联调的customerId和自己的联调服务地址，和前面自测的联调服务一致
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/10.png)
**注：** 
- 1.如果是ERP发起的，联调直接通过奇门上的测试工具，选择API名称，运行环境，appkey,secert还有wms的appkey,联调customerId,以及请求报文
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/11.png)
- 2.如果是wms进行回写，需要确认一下返回的数据格式是否无误，由wms那边调用联调服务地址进行回写

###### **7.奇门配置**

9.关于联调中QiMenClient地址配置
测试地址: [http://qimen.api.taobao.com/router/qmtest]([http://qimen.api.taobao.com/router/qmtest)
正式地址: [http://qimen.api.taobao.com/router/qimen/service](http://qimen.api.taobao.com/router/qimen/service)

###### **8.问题咨询**

10.过程中遇到问题如何解决?
1.提工单: [http://open.taobao.com/support/index.htm?spm=a219a.7386653.0.0.d467669ayt8Fff](http://open.taobao.com/support/index.htm?spm=a219a.7386653.0.0.d467669ayt8Fff)
2.加入钉钉群咨询
![Image text](https://raw.githubusercontent.com/jiubanmoli/image/master/12.png)


#### **10.目录结构:**
```
|——BMP-Project                --------整个项目的父模块
|   |——config                 --------项目配置文件
|   |——docx                   --------项目相关文档
|   |——px-bmp-auth            --------微服务认证服务器
|   |——px-bmp-common          --------通用模块
|   |   |——common-core        --------系统通用配置和工具类
|   |   |——common-datasource  ---------通用数据权限自动装配starter
|   |   |——common-doc         ---------文档模块的核心依赖包
|   |   |——common-doc-gateway ---------网关聚合微服务子系统api文档自动装配starter
|   |   |——common-doc-starter ---------微服务子系统api文档自动装配starter
|   |   |——common-logging     ---------微服务日志自动装配starter
|   |   |——common-redis       ---------微服务缓存自动装配starter
|   |   |——common-security    ---------微服务子系统安全配置自动装配starter
|   |   |——common-websocket   ---------微服务消息通知自动装配starter
|   |——px-bmp-gateway         ---------微服务网关
|   |——px-bmp-modules         ---------微服务子系统
|   |   |——px-bmp-base        ---------微服务子系统基础数据模块
|   |   |——px-bmp-erp         ---------微服务子系统ERP模块
|   |   |——px-bmp-order       ---------微服务子系统OMS模块
|   |   |——px-bmp-generator   ---------微服务子系统代码生成模块
|   |   |——px-bmp-chain       ---------微服务子系统WMS模块
|   |   |——px-bmp-job         ---------微服务子系统任务调度模块
|   |   |——px-bmp-user        ---------微服务子系统系统管理模块
|   |——px-bmp-monitor         ---------微服务监控系统
|   |——px-bmp-tx-manager      ---------微服务分布式事务控制器
```