# 痞子衡嵌入式半月刊： 第 113 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 112 期》](https://www.cnblogs.com/henjay724/p/18583038)

## 唠两句

历史上的今天：。

本期共 2 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、JesFs - 专门为小型低功耗设备设计的文件系统</font>

JesFs（Jo's Embedded Serial File System）是一款专为资源受限的嵌入式系统设计的轻量级串行 NOR 闪存文件系统。它具备极小的内存占用、强大的安全性以及优异的性能，完美适用于各种物联网应用场景，例如数据采集、事件记录和固件更新等。

 * 项目地址：https://github.com/joembedded/JesFs

JesFS 的一个基本特性是：可以把嵌入式系统的文件通过互联网自动地镜像存储到服务器，服务器因此具有嵌入式文件系统的一个实时更新的副本。这个特性也可以用在分钟级获取数据的场景，但是为了降低功耗，一般不会频繁通过互联网对比更新服务器副本（通常几小时一次）。 即使传输了新文件、远程升级了固件，只要有需要，JesFS 就可以通过特殊标志位（时间戳和 CRC32 哈希校验）很容易地从服务器上找回文件。

### <font color="red">2、Spiffs - 专门为嵌入式设备设计的轻量级文件系统</font>

Spiffs (SPI Flash File System) 是一个专门为嵌入式目标上的 SPI NOR 闪存设备设计的轻量级文件系统。它针对小型嵌入式设备的特点进行了优化，特别是在内存资源有限的情况下表现出色。Spiffs 的设计目标是：在最小化 RAM 使用量的同时，提供 POSIX 风格的 API 接口，方便开发者使用。

 * 项目地址：https://github.com/pellepl/spiffs

Spiffs 的主要功能包括：

```text
• 极低的RAM占用： Spiffs的设计理念是最大限度地减少RAM的消耗，它使用静态大小的RAM缓冲区，与文件数量无关，非常适合内存资源紧张的嵌入式系统。
• 类POSIX API： Spiffs提供了一套与POSIX标准兼容的API接口，包括open、close、read、write、seek、stat等常用函数，方便开发者快速上手和进行移植。
• 跨平台兼容性： 理论上，Spiffs不仅可以运行在SPI闪存上，也可以运行在微处理器的其他嵌入式闪存上，具有良好的平台兼容性。
• 多配置支持： 在同一个目标设备上，甚至在同一个SPI闪存设备上，可以运行多个Spiffs配置，灵活地管理不同的数据存储空间。
• 静态磨损均衡： Spiffs内置了静态磨损均衡算法，可以有效地延长闪存的使用寿命。
• 文件系统一致性检查： Spiffs具备内置的文件系统一致性检查机制，确保数据的完整性和可靠性。
• 高可配置性： Spiffs提供了丰富的配置选项，可以根据实际需求进行定制。
```

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-113/.PNG)


### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

