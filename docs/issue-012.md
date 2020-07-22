# 痞子衡嵌入式半月刊： 第 12 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 11 期》](https://www.cnblogs.com/henjay724/p/13258113.html)

## 唠两句


本期共收录 3条资讯、1个项目、1个工具、1个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、安谋中国自研第一代星辰处理器(STAR-MC1)正式商用</font>

日前，安谋中国宣发了一个重磅产品 - “星辰”第一代产品STAR-MC1，主要为满足AIoT应用性能、功耗、安全方面而生。

> 星辰处理器主页: https://www.armchina.com/Stars.html

Armv8-M架构是Arm去年下半年更新的最新架构，STAR-MC1是第一个对新架构实现的产品。除了Armv8-M的所有特色以外，需要注意的是STAR-MC1进一步拓展了TrustZone这一安全功能。STAR-MC1的创新性还在于整个缓存（Cache）的结构引入了M级别的处理器中，这种特色可充分提高系统级的性能和效率。

![](http://henjay724.com/image/biweekly/STAR-MC1.PNG)


目前STAR-MC1已有很多客户采用，并已取得流片，截至目前，星辰处理器已有30个授权客户，这30个授权客户里有21个客户已经有项目进行集成、设计，其中有7个项目已流片，广泛应用于通用MCU、互联芯片、系统控制、汽车电子、存储、定位、传感器控制等领域。

### <font color="red">2、Imagination推出汽车行业最先进GPU IP产品 - XS GPU</font>

近日， Imagination Technologies宣布推出面向汽车领域的XS图形处理器（GPU）产品系列，可实现先进驾驶辅助系统（ADAS）加速和安全关键图形处理功能。XS是迄今为止所开发的最先进的汽车GPU知识产权（IP），并且是业界首款符合ISO 26262标准的可授权IP，该标准旨在解决汽车行业中存在的功能安全风险。 

> 产品主页: https://www.imgtec.com/powervr-automotive/

XS GPU主要包括以下的一些特性：

```text
- ADAS计算加速：XS产品系列专门针对ADAS加速进行了优化，可提供高性能且具备 功能安全性的计算能力。
- 安全关键图形处理：XS是业界首个专为安全关键图形处理应用而设计的GPU产品系列，在这些应用中GPU负责数字仪表盘、全景环绕和摄像系统等关键任务。
- ISO 26262流程一致性：XS是汽车行业首款符合ISO 26262标准的GPU IP。整车厂（OEM）、一级供应商（Tier 1）和半导体供应商现在可以深具信心地将符合ISO 26262标准的IP集成至其产品中
```

![](http://henjay724.com/image/biweekly/Imagination-XS-GPU.jpg)

随着汽车系统的复杂度不断提升，功能安全的相关要求也开始越来越高。XS GPU的新型安全架构包含了正在申请专利的技术，该技术使Imagination能够验证和确保GPU数据的正确执行和传输。除锁步（lockstep）机制外，XS还包括硬件机制，可以在计算和图形处理功能上执行安全关键工作负载，同时实现性能最大化。 

### <font color="red">3、基于NXP i.MXRT的可刷脸的智能门锁来了！</font>

在近日举办的第22届中国广州国际建筑装饰博览会上，恩智浦半导体和深圳深岚科技视觉科技联合打造的最新人脸识别智能门锁亮相。

> 资讯主页: https://mp.weixin.qq.com/s/PCwEEUUYbPC7rVSVInpkZQ

![](http://henjay724.com/image/biweekly/NXP-106F.PNG)

随着物联网市场需求的变革，智能人脸识别方案也遇到了井喷式的发展。基于NXP i.MX RT106F的智能人脸识别方案在硬件上省去传统MPU+PMIC组合，替换昂贵的DDR，极大降低产品成本。软件上引入NXP的OASIS-LITE引擎， 使得整体性能比CMSIS-NN具有更高的准确性，速度和内存消耗上比TensorFlow-Lite更有优势。

该人脸识别方案能够完全脱机工作，对于未知新用户，可在不访问云端的情况下，在不到一秒钟的时间内识别出来，效果如下：

![](http://henjay724.com/image/biweekly/NXP-face.PNG)


## 项目类

### <font color="red">1、IOTQQ - 一个跨平台QQ机器人</font>

IOTQQ是一款跨平台的QQ机器人项目，适用于MAC平台、树莓派、路由器、电视盒子N1等。

> 项目主页: https://github.com/IOTQQ/IOTQQ

项目有主要以下特点：

```text
1.采用独特的插件机制--Lua
2.提供WebSocket（SocketIO）
3.提供Web API
4.内置协程池，高效，稳定，迸发
5.完成了大部分核心接口 其他必要接口持续更新
6.不断电稳定运行0崩,错误日志记录于log中体现
```

话不多说，运行效果直接上图：

![](http://henjay724.com/image/biweekly/IOTQQ_mac.PNG)

![](http://henjay724.com/image/biweekly/IOTQQ_shumeipai.PNG)

## 工具类

### <font color="red">1、EIDE - 一款能使vscode支持MCU开发的插件</font>

EIDE即Embedded IDE，这是一款由网友github0null开发并维护的应用于在vscode上提供对8051，STM8，Cortex-M项目进行开发，编译，烧录的功能的插件。

> 项目主页: https://github.com/github0null/eide 

该插件的功能特性如下：

```text
- 提供丰富的项目模板方便快速开始项目
- 支持从标准的CMSIS Package安装芯片的外设库
- 一键编译、快速编译，支持多种主流的编译工具
- 一键烧录到芯片，支持多种主流的烧录器
- 内置的串口监视器
- 为调试器Cortex-debug/STM8-debug自动生成调试配置
```

![](http://henjay724.com/image/biweekly/EIDE.png)

vscode作为当下非常流行的码农编辑器，嵌入式er们利用这款插件也能使用这款明星IDE进行MCU项目的开发啦。

## i.MXRT出品

### <font color="red">1、迈瑞医疗 - 心电除颤仪BeneHeart C系列</font>

这款心电与除颤仪具有智能易用（7＂彩色大屏，ResQNavi ™，开盖即开机，支持中英双语）、快速有效（QShock™，360J双相波）、可靠耐用（1.5米六面抗跌落，IP55防尘防水）、省心互联（AED-Alert™ 2.0-IoT远程设备管理，无需人工巡检）四大优点。

> RT芯片：i.MXRT1052
> 产品主页： https://www.mindray.com/cn/product/BeneHeart_C%E7%B3%BB%E5%88%97.html
> 参考售价： 未知

![](http://henjay724.com/image/biweekly/Mindary_BeneHeartC.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


