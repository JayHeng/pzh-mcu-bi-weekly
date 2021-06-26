# 痞子衡嵌入式半月刊： 第 34 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 33 期》](https://www.cnblogs.com/henjay724/p/14879976.html)

## 唠两句

这周一是夏至，历史上的今天：1997年6月26日，英国魔幻文学作品《哈利波特1 - 神秘的魔法石》出版。

本期共收录 2条资讯、3个项目、2个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、首届 RISC-V 中国峰会在上海举行</font>

首届RISC-V中国峰会（RISC-V World Conference China）于6月21日在上海科技大学盛大开幕。此次峰会线下超过1000人、线上超过10000人参会，超过100家厂商进行演讲或参展，是国内迄今为止规模最大的以RISC-V为主题的峰会。这也是RISC-V第一次在北美以外地区举办同等规模的峰会。

> 会议议程： https://www.riscv-conf-china.com/cn/agenda.html

![](http://henjay724.com/image/biweekly20210626/RISC-V_World_Conference_China_1st.PNG)

### <font color="red">2、中科院计算所公布开源 RISC-V 处理器核心 - 香山</font>

中国科学院计算技术研究所的包云岗团队推出了一款开源的高性能 RISC-V 处理器 - 香山，该核心基于 Chisel 硬件设计语言实现，支持 RV64GC 指令集。香山共有两版微架构，第一版叫雁栖湖，第二版叫南湖。

> 项目主页：https://github.com/OpenXiangShan/XiangShan

雁栖湖是一个11级流水、6发射、4个访存部件的乱序处理器核，该架构的频率可以达到1.3GHz@TSMC 28nm，性能预计可以达到 7 分 / GHz（SPEC CPU 2006）。南湖的设计目标更高：频率期望达到 2GHz@SMIC 14nm，性能期望达到 10 分 / GHz（SPEC CPU 2006 ）。

![](http://henjay724.com/image/biweekly20210626/Xiangshan_yanxihu.PNG)

## 项目类

### <font color="red">1、RT-FOTA - 基于 STM32 的开源 Bootloader 框架</font>

RT-OTA 是 RT-Thread 官方推出的 STM32 系列单片机的通用 bootloader（商用性质，不公开源码），而 RT-FOTA 可以理解为是 RT-OTA 项目的民间开源版，由王希个人维护。  

> 项目主页：https://gitee.com/spunky_973/rt-fota

RT-FOTA 主要的功能：

```text
1. 支持 RTT 官方的 RBL 打包软件，使用方式也一致。目前支持包括 CRC32、AES256、quicklz 和 fastlz 功能；
2. 支持命令行模式（FINSH 组件）和出厂固件恢复；
3. 支持 FLASH 分区（FAL 组件）；
4. 支持功能扩展（RTT 组件）；
5. 其他功能可自行方便扩展；
```

![](http://henjay724.com/image/biweekly20210626/RT-FOTA.PNG)

### <font color="red">2、RanFS - 一个轻量级的嵌入式文件系统库</font>

RanFS是基于C(C89)编写的，提供POSIX兼容的文件操作API，轻量级的文件系统库。RanFS目标是为嵌入式设备提供功能完善和高效的文件操作API，通过上层接口封装实现对多种文件系统的读写或读支持。

> 项目主页：http://www.ranfs.com/cn/?RFS

RanFS可运行在资源很少的单片机环境里，比如 8051, PIC, AVR, ARM, DSP, Z80, 78K 等等。RanFS目前支持 fat12/16/32 可读写文件系统，ntfs、ext2、ext3、ext4可读文件系统，支持大于512字节扇区的盘，支持超过2T的硬盘，支持多分区 多文件，支持长文件名打开、创建、删除，支持通过扇区偏移量快速打开文件，支持创建目录等等。

![](http://henjay724.com/image/biweekly20210626/RanFS.PNG)

### <font color="red">3、SimpleGUI - 一款针对单色显示屏设计的GUI接口库</font>

SimpleGUI是一套针对单色显示屏的可拓展嵌入式的开源GUI解决方案，提供了各种常用界面元素的绘制接口与一个简练的HMI交互引擎，此外还包含一个简易LCD模拟器，带有截图保存和复制功能， 用户也可以在模拟环境中模拟自己需要的处理逻辑。

> 项目主页：https://gitee.com/Polarix/simplegui

SimpleGUI 在尽可能减小资源消耗的前提下，提供以下功能：
```text
1. 点、线、基本几何图形、单色位图、文字等的绘制功能。
2. 列表、进度条、滚动条、提示框、曲线图等部件的设置元显示功能。
3. 单色显示屏模拟环境，方便脱离硬件平台进行部分GUI开发。
```

![](http://henjay724.com/image/biweekly20210626/SimpleGUI.PNG)

SimpleGUI的LCD模拟器基于wxWidgetsGUI框架开发。系统工程CodeBlocks集成开发环境与MinGW编译器搭建。

![](http://henjay724.com/image/biweekly20210626/SimpleGUI_sim.PNG)

## 工具类

### <font color="red">1、CLion - 专为 C/C++ 而生的跨平台 IDE</font>

CLion是JetBrain出品的一款专为开发C及C++所设计的跨平台IDE，它以IntelliJ为基础设计，包含了许多智能功能来帮助开发人员在Linux、OS X和Windows上来开发C/C++，同时它还使用智能编辑器来提高代码质量、自动代码重构并且深度整合CMake编译系统，从而提高开发人员的开发效率。

> 软件主页：https://www.jetbrains.com/zh-cn/clion/promo/

![](http://henjay724.com/image/biweekly20210626/CLion.PNG)

### <font color="red">2、TabNine - 最好的代码自动补全工具</font>

这是来自加拿大的学霸 Jacob Jackson 开发的一款”Deep TabNine“代码补全工具，它支持23种编程语言（Java/Python/C++等等）、5种编辑器(VS Code/Sublime Text/Atom/Emacs/Vim)，使用简单，效果惊艳。不少使用过的网友都说：TabNine是他们用过的最好的代码补全工具，这是属于程序员的杀手级应用。

> 软件主页：https://www.tabnine.com/

![](http://henjay724.com/image/biweekly20210626/TabNine.gif)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

