# 痞子衡嵌入式半月刊： 第 118 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 117 期》](https://www.cnblogs.com/henjay724/p/18708118)

## 唠两句

历史上的今天：。

本期共 1 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、IMU_Array- 全开源32路IMU传感器矩阵列</font>

这个项目使用 iCE40 接了 32 路 IMU 传感器。使用 IMU 可以知道自己相对于地球的位置。它们本质上是机械设备，因此并非万无一失。一种引起关注的方法是将多个 MEMS IMU 放在单个 PCB 上，将其连接到 FPGA，然后将它们的数据一起处理，以获得更灵敏的 IMU 或过滤漂移。当前代码没做任何花哨的数据处理，只是读取 32 个 IMU 数据，或者发送所有数据，或者做一个简单的平均（实际上只是累积）并输出结果（它处理 IMU 的 4 个不同旋转）。

 * 项目地址：https://github.com/will127534/IMU_Array

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-118/IMU_Array.png)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

