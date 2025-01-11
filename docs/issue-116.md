# 痞子衡嵌入式半月刊： 第 116 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 115 期》](https://www.cnblogs.com/henjay724/p/18631487)

## 唠两句

历史上的今天：

本期共 1 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、CosyOS - 零中断延迟的RTOS</font>

CosyOS 是一款来自中国的开源实时操作系统，从经典的 8051 内核，到流行的 Arm Cortex-M 内核，均可实现全局不关总中断、零中断延迟，适用于对系统实时性及中断响应速度有较高要求的场合。CosyOS 以极具浪漫主义色彩的宏定义，实现了高度的面向对象及良好的易用性。CosyOS 以零中断延迟为宗旨，突破创新为方针，简单易用为原则。

 * 项目地址：https://gitee.com/cosyos/cosyos

CosyOS 零中断延迟基本原理：

```text
- 服务层中，SysTick、PendSV、任务临界区，三者间是互斥访问的。换言之，整个服务层是一个大临界区（服务层临界区）。
- 所有内核服务（中断本地服务除外），均在 “服务层临界区” 执行，从而保证服务的 “操作流” 不会被打断。
- 中断本地服务采用互斥访问机制。
```

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-116/.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

