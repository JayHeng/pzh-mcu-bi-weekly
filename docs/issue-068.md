# 痞子衡嵌入式半月刊： 第 68 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 67 期》](https://www.cnblogs.com/henjay724/p/16920757.html)

## 唠两句

历史上的今天：。

本期共收录 2 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、USB Cable Tester - 各种接口类型USB电缆的便携测试仪</font>

网友 alvarop 制作的一块板卡，能够测试各种 USB 线是否完好。(注意USB标准有助于识别板卡上的这些USB- c，符合标准的电缆将根据电缆和连接器规格发布选择合适的引脚)。将测试的 USB 线连接到板子两侧，如果对应线是通的，那板子上的信号 LED 将被点亮。

> * 项目地址：https://github.com/alvarop/usb_c_cable_tester

![](http://henjay724.com/image/biweekly20221211/usb_c_cable_tester.PNG)

### <font color="red">2、ECBM - 基于STC8系列的外设函数库</font>

ECBM 工作室为 STC8 单片机设计的外设函数库（当前是 V3 版本），目前已经支持 STC8 全型号，外设部分会逐渐完善。STC8 是目前 51 单片机里最好用的系列，拥有最多 8K 的SRAM、64K 的Flash、5个定时器、4个串口。全系列都带IIC和SPI，大部分带ADC。STC8H还带有硬件USB。

ECBM 工作室在推广 ECBM 库 V3 的过程中，用户反馈 ECBM 占用空间太大，新手对库不了解不知道怎么优化，于是、专门推出官方优化精简版！在保证了 ecbm 特色的情况下，去除大量用不到的鸡肋功能，只为了核心和精简而存在的STC8库。

> * 项目地址1：https://gitee.com/ecbm/ecbm_library
> * 项目地址2：https://gitee.com/ecbm/ecbm-library-lite

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

