# 痞子衡嵌入式半月刊： 第 116 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 115 期》](https://www.cnblogs.com/henjay724/p/18631487)

## 唠两句

历史上的今天：

本期共 3 个项目，希望对你有帮助！

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

### <font color="red">2、EFSMC - 一个基于事件驱动的有限状态机</font>

EFSM (event finite state machine，事件驱动型有限状态机)，是一个基于事件驱动的有限状态机，主要应用于嵌入式设备的软件系统中。

 * 项目地址：https://gitee.com/simpost/EFSMC

EFSM 的设计原则是：简单！EFSM 的使用者只需要关心：

```text
- 当事件到来时，通过EFSM取得对应事件的处理方法；
- 当特定事件到来，或者条件满足时，调用状态切换方法进行状态切换。
```

由于 EFSM 的巧妙设计，避免了命名冲突的问题，用户可以在一个程序中定义多个状态机；要是能对不同状态进行组织，还可以做出层次状态机的结构。

### <font color="red">3、eLab - 集成多种开源项目和多个技术特性的嵌入式开发平台</font>

eLab 是一个集成了多种开源项目和多个技术特性的嵌入式开发平台。作者在这个项目里汇集了多年来在产品开发中的开发理念和经验，以现有的开源软件为主，以作者自己开发的组件为辅，打造一个统一而完善的开发平台。

 * 项目地址：https://gitee.com/event-os/elab

eLab 项目，侧重两大技术方向，一是产品级的嵌入式软件开发，二是跨平台的嵌入式软件开发。这两个技术方向，最终目的，都是为了让工程师的开发效率，得到颠覆性的提升。尤其很多非软件或者非计算机专业毕业的嵌入式工程师们，不必在错误或者跑偏的技术方向上苦苦探索，从而减少技术进阶的年限，早日进入更高的职业阶段。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-116/.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

