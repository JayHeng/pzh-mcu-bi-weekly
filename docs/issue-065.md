# 痞子衡嵌入式半月刊： 第 65 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 64 期》](https://www.cnblogs.com/henjay724/p/16755687.html)

## 唠两句

历史上的今天：

本期共收录 2 个项目、0 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、zBitsView - 单片机实现多层菜单的屏幕界面</font>

zBitsView 是一个基于单片机实现的多层菜单的屏幕界面。硬件原型：STM32F103C8T6、Nokia 5110屏幕，EC11旋转编码器，但是界面控件理论上不限制屏幕、不限制单片机型号，移植非常方便。  

> * 项目地址：https://github.com/figght/zBitsView

使用 zBitsView 设计菜单界面时只需要定义几个数组。首先定义 RowListTypeDef 类型数组，根据界面数定义数组个数，根据每个界面包含的行元素数定义每个数组的长度。然后定义 ViewListTypeDef 类型数组，定义一个即可，数组长度是界面数决定的。

![](http://henjay724.com/image/biweekly20221023/zBitsView.PNG)

### <font color="red">2、FreeEEG32 - 开源EEG脑电图参考设计</font>

FreeEEG32 是一种可堆叠的，开源的，32通道，24位，sigma-delta，多路采样板，旨在满足科学家和大脑黑客的需求。FreeEEG32 结合了 4 个 8 通道 AD7771，主控是 STM32H7。它足够敏感，可以处理高质量的脑电图数据采集。  

> * 项目主页：https://www.crowdsupply.com/neuroidss/freeeeg32

为了满足 EEG 标准，FreeEEG32 的固件在同时运行所有 32 个通道时优化为每个通道 512SPS。通过堆叠 FreeEEG32 板，可以实现 64-256 通道的同步流。每块板独立地连接到主机，但可以流到相同的软件实例进行大量数据收集。  

![](http://henjay724.com/image/biweekly20221023/FreeEEG32.PNG)

FreeEEG32 与市面上其它 EEG 参考板的比较：

![](http://henjay724.com/image/biweekly20221023/FreeEEG32-2.PNG)

## 工具类


### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

