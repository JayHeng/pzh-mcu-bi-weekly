# 痞子衡嵌入式半月刊： 第 15 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 14 期》](https://www.cnblogs.com/henjay724/p/13547256.html)

## 唠两句

今天是白露，时至白露，基本结束了暑天的闷热，天气渐渐转凉，它是秋季中闷热转向凉爽的转折节点。

痞子衡昨天在微信公众号写了第一篇个人职场感悟系列，没想到反响还不错，接下来痞子衡会继续把更多的感悟陆续写出来，语言一如既往平实，绝对亲身经历，希望对大家在未来的职场上有所启发。

本期共收录 2条资讯、2个项目、2个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、华虹半导体最新推出90纳米超低漏电嵌入式闪存工艺平台助力大容量MCU解决方案</font>

近日，晶圆代工厂商华虹半导体宣布推出90纳米超低漏电eFlash及EEPROM工艺平台，满足大容量微控制器的相关需求。

> 资讯主页: https://www.huahonggrace.com/c/news.php

该工艺平台具有以下特点：

```text
- 1.5V核心N型和P型MOS晶体管漏电达到0.2pA/μm，有效延长MCU待机时间
- eNVM IP具有10万至50万次擦写次数，读取速度达30ns
- 400Kgate/mm2以上的高逻辑单元集成度，有助于缩小芯片面积
- 同时支持RF、eFlash及EEPROM
```

![](http://henjay724.com/image/biweekly/Huahong_90nm_eFlash.png)

该工艺平台作为华虹半导体0.11微米超低漏电技术的延续，以更低的功耗和成本为芯片设计厂商提供具有竞争力的差异化解决方案，适用于物联网、可穿戴式设备、工业及汽车电子等方面的应用。 

### <font color="red">2、瓴盛科技发布首款AIoT芯片 - JA310</font>

> 资讯主页: http://www.eepw.com.cn/article/202008/417677.htm

近日，瓴盛科技在成都召开了“芯视觉”产品发布会，推出了瓴盛首颗AIoT SoC产品JA310。

这颗JA310芯片具有以下特点：

```text
- 采用三星11nm FinFET工艺，相比三星的28nm工艺，功耗下降70%
- 采用四核ARM Coterx-A55内核，主频达到1.5GHz
- 集成AI专用NPU，支持INT16/FP16、支持TensorFlow/Caffe2等框架，算力可达2TOPS
- 集成专业及安防ISP及高品质低延时VPU
```

![](http://henjay724.com/image/biweekly/JLQ_JA310.png)

这颗JA310主要面向智慧监控、人脸识别、视频会议、车载终端、运动相机等广泛的智慧物联网应用。 

## 项目类

### <font color="red">1、Simple Dynamic Strings - 一个增强的C字符串处理库</font>

Simple Dynamic Strings (简称 SDS) 是一个 C 语言字符串库，旨在通过添加堆分配的字符串来增强有限的libc字符串处理功能。

> 项目主页： https://github.com/antirez/sds

SDS设计中没有使用C结构来表示字符串，而是使用存储在SDS返回给用户的字符串的实际指针之前的二进制前缀。

![](http://henjay724.com/image/biweekly/Simple_Dynamic_Strings.PNG)

SDS 特点如下：

```text
- 使用更简单;
- 二进制安全;
- 效率更高;
- 与 C 字符串函数兼容;
```

SDS是作者过去为满足日常C编程需要而开发的一个C字符串，后来它被移到Redis中，在那里它被广泛使用，并在那里进行了修改以适合高性能操作。现在它是从Redis中提取出来的，并作为一个独立的项目分叉。

### <font color="red">2、PLOOC - 一组经过精心打磨的C宏模板</font>

PLOOC是ARM大神王卓然（江湖绰号傻孩子）维护的项目，它是一组经过精心打磨的C宏模板，为私有类成员提供保护。该模板充分利用了ANSI-C强制编译规则，以最少的成本提供所需的OO特性。

> 项目主页： https://github.com/GorgonMeducer/PLOOC

PLOOC 特点如下：

```text
- 支持受保护的成员
- 支持多重继承
- 支持接口实现
- 在某些编译器中支持严格的类型检查/验证，例如启用了多文件编译的IAR。
- 符合ANSI-C99
- 也支持ANSI-C90，但对私有功能的保护被禁用。
- 支持过载
- 需要C11或_Generic
- 低开销
```

## 工具类

### <font color="red">1、Q-Dir - 实用的多窗口资源管理器</font>

> 工具主页: http://q-dir.com

大多数嵌入式er们的开发工作，都是在Windows环境下进行的，而工作时打开分布在各个不同文件夹的工程、文档、软件的频率是相当高的，windows本身自带的资源管理器在进行多文件夹操作时极其不方便。这款Q-Dir软件作为一个多窗口资源管理器包含了windows自带资源管理器的所有功能，还附加了许多额外功能，亲爱的嵌入式er们值得拥有。

Q-Dir有如下的一些特点：

```text
- 快速访问常用文件夹
- 窗口间文件拖拽
- 文件及文件夹过滤器
- 允许快速预览
- 多语言支持
```

![](http://henjay724.com/image/bi-weekly/Q-Dir.png)

### <font color="red">2、MobaXterm - 满足你所有要求的终端神器</font>

MobaXterm是一款免费的适用于Windows的增强型终端，带有X11服务器，选项卡式SSH客户端，网络工具等多重功能。

> 软件主页: https://mobaxterm.mobatek.net/

MobaXterm具有如下的功能特点：

```text
- 基于X.org的完全配置的Xserver
- 从Windows显示远程Unix界面
- 多功能会话管理器
- 支持SSH, X11, RDP, VNC, FTP, MOSH等远程网络工具
- 支持添加插件扩展更多功能
```

![](http://henjay724.com/image/bi-weekly/MobaXterm.gif)

对于嵌入式er来说，MCU开发中常用到的串口工具，MPU开发中常用的远程终端，或者是嵌入式玩家想要利用SSH连接类似Raspberry Pi的开源硬件等功能，MobaXterm都能提供很好的支持。

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


