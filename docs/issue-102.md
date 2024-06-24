# 痞子衡嵌入式半月刊： 第 102 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 101 期》](https://www.cnblogs.com/henjay724/p/18214344)

## 唠两句

历史上的今天：1991年6月24日，中国首座脉冲反应堆建成。

本期共 4 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、eepromfs - 基于EEPROM的简易类文件数据读写库</font>

eepromfs 是一个基于 EEPROM 的简易类文件的数据读写库，方便做动态功能增减时参数管理，增减参数块类似增减文件，不会对已有数据存储带来影响，适合在 EEPROM 硬件资源充裕的情况下使用。

该库设计的核心思想是 EPPROM 存储区开头存储 eepromfs 管理相关信息，采用链表方式串联每一个文件，每个文件建立的时候指定名称和大小，新增加的文件自动追加在链表末尾。该科可以在大部分嵌入式 arm 下使用，硬件需要带 eeprom，建议采用 24C256、24c512 之类的大容量芯片。

 * 项目地址：https://gitee.com/wtau_zaozao/eepromfs

### <font color="red">2、PDHV - 可调高压USB PD电源</font>

PDHV 是一个可调 300V 高压 USB PD 电源，所有 USB 端口都彼此隔离并与高压隔离。

 * 项目地址：https://github.com/Aylo6061/PDHV

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-102/PHDV.PNG)

 ### <font color="red">3、Modular-Things - 基于OSAP协议实现的简化硬件设计</font>

Modular-Things 项目是一种构建可在软件中组成的模块化硬件系统的方法。底层技术是一个小型网络库，用于跨设备打包和路由消息(OSAP)，以及一个基于 web 的编辑器，用于将硬件组合成软件中的功能系统。

Modular-Things 项目可以让你使用硬件设备，并为其添加一个库，该库允许你将该设备插入基于浏览器的编辑器中，在那里你可以编写控制它和其他设备的程序。因为它是浏览器中的 JavaScript，所以你也可以用 HTML/CSS/JS 编写接口，并导入各种与物理计算系统交互和控制的高级库。

 * 项目地址：https://github.com/modular-things/modular-things

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-102/Modular-Things.PNG)

 ### <font color="red">4、OpenEarable - 基于Arduino的入耳式传感应用平台</font>

OpenEarable 是一个新的、开源的、基于 Arduino 的基于耳朵的传感应用平台。它提供了一个多功能的原型平台，支持各种传感器和执行器，使其适合耳式研究和开发。  

 * 项目地址：https://github.com/teco-kit/open-earable

OpenEarable 旨在通过提供灵活的开源硬件平台来实现基于耳朵的传感应用。它集成了一系列传感器，包括一个 9 轴惯性测量单元，一个耳道压力和温度传感器，一个向内超声波麦克风，一个扬声器，一个按钮和一个可控的 RGB LED。通过这些特性，OpenEarable 为研究人员和开发人员提供了探索各种应用场景的能力。

OpenEarable 通过 BLE (低功耗蓝牙)控制和传输传感器数据。音频播放和记录到内部 SD 卡(所需卡SanDisk Extreme Class 3，必须格式化为 exFAT)。OpenEarable 与提供的仪表板和 edge-ml 兼容。

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-102/OpenEarable.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

