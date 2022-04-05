# 痞子衡嵌入式半月刊： 第 52 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 51 期》](https://www.cnblogs.com/henjay724/p/16064331.html)

## 唠两句

明天是清明，历史上的今天：1815年4月5日，印度尼西亚坦博拉火山喷发，是人类历史上有记载的最猛烈火山爆发事件。

本期共收录 2个项目、0个工具，希望对你有帮助！

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

### <font color="red">2、Opus - 高灵活度的开源音频编解码器</font>

Opus 是用 C 语言开发的一个高灵活度的音频编码器，针对 ARM、x86 有特殊优化。Opus 在各方面都有着明显优势，它同时支持语音与音乐的编码，融合了 SILK 编码方法和 CELT 编码方法。SILK 原本被用于 Skype 中，基于语音信号的线性预测分析（LPC），对音乐支持并不好。而 CELT 尽管适用于全带宽音频，但对低比特率语音的编码效率不高，所以两者在 Opus 中形成了互补。

> * 项目主页：https://www.opus-codec.org/

![](http://henjay724.com/image/biweekly20220404/Opus.PNG)

Opus 特点包括：

```text
1. 比特率从 6kb/s 到 510 kb/s
2. 采样率从 8kHz（窄带）到 48kHz（全频段）
3. 帧大小从 2.5ms 到 60ms
4. 支持恒定比特率（CBR）和可变比特率（VBR）
5. 从窄带到全频带的音频带宽
6. 支持语音和音乐
7. 支持单声道和立体声
8. 支持多达255个通道（多流帧）
9. 动态可调比特率，音频带宽和帧大小
10. 良好的稳健性和隐蔽性
11. 浮点和定点实现
```

## 工具类


### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

