# 痞子衡嵌入式半月刊： 第 42 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 41 期》](https://www.cnblogs.com/henjay724/p/15389996.html)

## 唠两句

下周六是霜降，历史上的今天：1990年10月17日，世界上第一家互联网数据资料库诞生，简称“IMDB”，在美国成立。

本期共收录 2个项目、3个工具、2个RT产品，希望对你有帮助！

## 项目类

### <font color="red">1、irtu-gps - 基于iRTU项目实现GPS数据的接收和展示</font>

irtu-gps 基于iRTU项目（一个开源的DTU/RTU解决方案，基于合宙硬件模块），实现了GPS数据的接收和展示，设备PCB开源/服务器端开源/小程序全开源。

> 项目主页： https://gitee.com/wendal/irtu-gps

技术特点:

```text
1. 基于smart-socket的高性能io框架,轻松支持10w设备同时在线
2. 直接支持iRTU内置的JSON注册包
3. 无缝支持GPS的json数据包和hex数据包, 推荐选用hex,节省流量,性能更高
4. 自动建表,自动初始化. 默认配置H2数据库, 无需额外安装. 可按需要使用其他数据库
5. 基于NutzBoot,单个jar即可运行, 无需web容器,内存占用最低可到48mb
6. 配套微信小程序 https://gitee.com/wendal/irtu-gps-miniapp
```

### <font color="red">2、u8g2_wqy - 适合 u8g2 图形库的中文字体</font>

u8g2_wqy 是适合 u8g2 的中文字体，采用文泉驿点阵宋体作为源本，提供 12x12、13x13、14x14、15x15 和 16x16 点阵字库。

> 项目主页： https://github.com/larryli/u8g2_wqy

## 工具类

### <font color="red">1、Jenkins - 最流行的开源免费持续集成工具</font>

Jenkins 是一个开源的、提供友好操作界面的持续集成(CI)工具，起源于Hudson（Hudson是商用的），主要用于持续、自动的构建/测试软件项目、监控外部任务的运行。

Jenkins 用Java语言编写，可在Tomcat等流行的servlet容器中运行，也可独立运行。通常与版本管理工具(SCM)、构建工具结合使用。

> 软件主页： https://www.jenkins.io/

![](http://henjay724.com/image/biweekly20211017/Jenkins_CI.PNG)

### <font color="red">2、Black Duck Protex - 知名的开源代码检测工具</font>

Black Duck 是最早进行开源代码检测工具开发的公司（2017年被 Synopsys 收购），Protex 平台是黑鸭子套件的重要组件，为用户提供细粒度（代码片段级别）和高精度的开源代码检测能力，它基于黑鸭子知识库（Knowledge Base，KB）进行工作，支持本地化部署使用。能够帮助用户：

```text
1. 检查软件代码，确认代码的组成成分
2. 了解各种代码组分的许可证（License）及其间的冲突
3. 掌握和管理其日益复杂的软件及License
4. 进行代码的合规性、同源性检查
```

> 软件主页： https://www.blackducksoftware.com/

![](http://henjay724.com/image/biweekly20211017/BlackDuckProtex.PNG)

### <font color="red">3、Coverity - 知名的代码静态检测工具</font>

Coverity 是一款快速、准确且高度可扩展的静态分析 (SAST) 解决方案（这家公司于2014年被 Synopsys 收购），可帮助开发和安全团队在软件开发生命周期 (SDLC) 的早期解决安全和质量缺陷，跟踪和管理整个应用组合的风险，并确保符合安全和编码标准。 

> 软件主页： https://scan.coverity.com/

Coverity 主页还记录了其检测出的大量知名项目里的潜在代码问题，代码片段全部列了出来，大家都可以去看看这些代码，对提升代码能力非常有帮助。 

> 典型案例： https://scan.coverity.com/o/oss_success_stories

## i.MXRT出品

### <font color="red">1、Amazfit - 智能手表 GTR 3</font>

Amazfit GTR 3 系列智能手表首次搭载华米科技自研的原生智能手表操作系统 Zepp OS，搭配新一代 BioTracker 3.0 PPG 生物追踪光学传感器，健康、运动、智能体验全面升级，释放智能手表全新可能。Amazfit GTR 3 采用经典圆形造型，搭载了一块 1.39 英寸视网膜级屏幕。

> RT芯片：i.MXRT535
> 产品主页： https://us.amazfit.com/products/amazfit-gtr-3
> 官网定价： 899 元起

![](http://henjay724.com/image/biweekly20211017/Amazfit_GTR-3.PNG)

### <font color="red">2、Amazfit - 智能手表 GTR 3 Pro</font>

在 GTR 3 基础上，Amazfit GTR 3 Pro 通过行业内领先的柔性技术和工程设计，将圆形手表屏占比提升到业内领先的 70.6%，黑边压缩到 3.5mm，最终在同样大小的机身上做到 1.45 英寸超大显示屏。GTR 3 Pro 还首次搭载 PumpBeats 血压监测引擎，并通过与北京大学第一医院合作，共同研究腕部智能血压手表在未诊断高血压人群中对高血压的筛查作用。

> RT芯片：i.MXRT595
> 产品主页： https://us.amazfit.com/products/amazfit-gtr-3-pro
> 官网定价： 1099 元起

![](http://henjay724.com/image/biweekly20211017/Amazfit_GTR-3-Pro.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

