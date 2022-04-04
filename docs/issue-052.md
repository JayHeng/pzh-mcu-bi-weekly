# 痞子衡嵌入式半月刊： 第 52 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 51 期》](https://www.cnblogs.com/henjay724/p/16064331.html)

## 唠两句

明天是清明，历史上的今天：1975年4月4日，美国微软公司创立。

本期共收录 1个项目、0个工具，希望对你有帮助！

## 项目类

### <font color="red">1、Qfplib - 专为ARM Cortex-M内核设计的浮点库</font>

Qfplib 是 ARM Cortex-M 内核的 IEEE 754 浮点库家族。Qfplib 有三个分支针对不同的内核，并以不同的优化目标编写。

```text
Qfplib-M0-tiny： 针对ARM Cortex-M0，高度优化的代码大小，仅单精度。
Qfplib-M0-full： 针对ARM Cortex-M0，优化了代码大小和速度，单精度和双精度。
Qfplib-M3： 针对ARM Cortex-M3，高度优化的速度，单精度。
```

> * 项目主页：https://www.quinapalus.com/qfplib.html

下表比较了 Qfplib-M3 与其他库的循环计数。 Qfplib-M3 计时结果是显示的参数值范围内的近似平均值，包括3个周期的调用开销。 它们是使用 LPC1763 微控制器从(单周期)RAM执行的：

![](http://henjay724.com/image/biweekly20220404/Qfplib.PNG)

## 工具类


### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

