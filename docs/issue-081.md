# 痞子衡嵌入式半月刊： 第 81 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 80 期》](https://www.cnblogs.com/henjay724/p/17711448.html)

## 唠两句

历史上的今天：

本期共收录 1 个项目、0 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、ESP32-Paxcounter - Wifi和BLE驱动的乘客流量测量仪</font>

Paxcounter是一个 proof-of-concept 设备，用于实时测量客流，它计算周围有多少移动设备，这可以估计出周围有多少人。Paxcounter检测空中的Wifi和蓝牙信号，通过过滤MAC地址中的供应商oui来关注移动设备。

这个项目的目的是在不侵犯隐私的情况下做到这一点：如果你只想统计用户拥有的设备，你不需要跟踪他们。因此，Paxcounter不会持久地存储MAC地址，也不会对扫描的设备进行指纹识别。数据通过LoRaWAN网络和/或有线SPI从接口传输到服务器。它也可以存储在本地SD-card上。

> * 项目地址：https://github.com/cyberman54/ESP32-Paxcounter

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-081/ESP32-Paxcounter.PNG)



## 工具类



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

