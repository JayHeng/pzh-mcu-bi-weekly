# 痞子衡嵌入式半月刊： 第 7 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 6 期》](https://www.cnblogs.com/henjay724/p/12728731.html)

## 唠两句

今天是立夏，夏季的第一个节气。

本期共收录 2条资讯、3个项目、2个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、GitHub 宣布向所有人免费开放所有核心功能</font>

近日，GitHub CEO Nat Friedman 在官方博客中正式宣布，GitHub 所有核心功能从此对所有人都免费提供。

> 消息来源: https://github.blog/2020-04-14-github-is-now-free-for-teams/

![](http://henjay724.com/image/biweekly/github_free_for_teams.png)

本次重大福利更新包括：

```text
1、此前仅对个人免费的私有仓库，现在对所有账号类型开放，取消协作者数量上限；
2、GitHub Pro 现在将包括 2GB 的 Packages 存储和 10GB 的数据传输；
3、在官宣时间之前注册并已为团队服务付费的用户，订单到期之日按比例退款；
4、自 5 月 14 日起，GitHub 团队每月将为私有仓库提供 3000 分钟的操作时间；
```

提及 GitHub，程序员中无论是新手，还是大神，无论秃顶的还是刚入行满头黑发的都应该知道。GitHub 中的有很多优质的代码可以参考。然而，GitHub并不是完全免费的，但现在 GitHub 又有了一项大动作，确实是程序员的一个相当好的福利。

### <font color="red">2、英飞凌并购赛普拉斯宣告完成，跃居全球第一车用半导体供应商</font>

近日，总部位于圣何塞的赛普拉斯半导体公司正式并入英飞凌科技股份公司，标志着英飞凌史上最大并购案宣告完成。新的英飞凌在汽车电子市场份额预计可达到 13％，一举超过竞争对手恩智浦成为最大的汽车芯片供应商。

> 资讯主页：https://www.infineon.com/cms/en/about-infineon/press/press-releases/2019/INFXX201906-074.html

![](http://henjay724.com/image/biweekly/Cypress_Infineon.PNG)

随着赛普拉斯的加入，英飞凌将进一步强化其结构性增长驱动，拓展更广泛的应用领域，以加速公司的盈利性增长。赛普拉斯的产品主要有微控制器、连接组件、软件系统以及高性能存储器等，与英飞凌领先的功率半导体、汽车微控制器、传感器以及安全解决方案，形成了高度的优势互补。赛普拉斯强大的研发能力以及在美国和日本市场上的稳固地位，也将为英飞凌的全球客户提供更有力的支持。

## 项目类

### <font color="red">1、BabyOS - 一套管理功能模块和外设驱动的 MCU 项目开发框架</font>

BabyOS 是由网友 notrynohigh 开发维护的适用于 MCU 项目的一套管理功能模块和外设驱动的框架。

> 项目主页: https://github.com/notrynohigh/BabyOS

对项目而言，使用 BabyOS 能缩短开发周期。项目开发时选择适用的功能模块及驱动。直接进入功能代码编写的阶段。对工程师而言，使用 BabyOS 能减少重复工作，调试过的功能模块和驱动代码放入 BabyOS 中进行管理，以后项目可以直接使用，去掉重复调试的工作。

![](http://henjay724.com/image/biweekly/BabyOS_framework.png)

### <font color="red">2、EasyFlash - 一款轻巧的嵌入式 Flash 存储器库</font>

EasyFlash是一款开源的轻量级嵌入式Flash存储器库，方便开发者更加轻松的实现基于Flash存储器的常见应用开发。非常适合智能家居、可穿戴设备、工控、医疗、物联网等需要断电存储功能的产品，资源占用极低，支持各种MCU片上存储器。 

> 项目主页: https://github.com/armink/EasyFlash 

该库主要有三大实用功能：

-  **ENV** 快速保存产品参数，支持 **写平衡（磨损平衡）**及 **掉电保护** 功能 
-  **IAP** 封装了IAP常用接口，同时支持Bootloader及Application的升级
-  **Log** 无需文件系统，日志可直接存储在Flash上 ，搭配EasyLogger，轻松实现 C日志的Flash存储功能 

![](http://henjay724.com/image/biweekly/EasyFlash.gif)

目前EasyFlash的最新版本V4.0支持了更多新特性，支持了增量升级、数据加密及压缩等功能，感兴趣的读者可以去项目主页一探究竟。

### <font color="red">3、</font>

## 工具类

### <font color="red">1、</font>

### <font color="red">2、千呼万唤始出来！IntelliJ IDEA 2020.1正式发布</font>

2020是JetBrains公司成立的第20个年头，4月9号，JetBrains发布了其新十年的首个版本 IntelliJ IDEA 2020.1，添加了对 Java 14 的支持、为部分 Web 和测试框架添加了新的功能，通过数据流分析辅助升级了调试器，新增了 LightEdit 模式，以及还支持从 IDE 直接下载和配置 JDK 的功能。最重要的是它还支持了中文，对于英文不好的同学来说是个很大的福利啊。话不多说，去它的下载主页尝尝鲜。

![](http://henjay724.com/image/biweekly/IntelliJ_2020.1.png)

> 下载主页: https://www.jetbrains.com/idea/whatsnew/?_ga=2.223997853.766751345.1587148177-1945597286.1562144217

