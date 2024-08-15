# 痞子衡嵌入式半月刊： 第 106 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 105 期》](https://www.cnblogs.com/henjay724/p/18314326)

## 唠两句

历史上的今天：

本期共 1 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、linux-ch32v003 - 在ch32v003单片机上运行Linux</font>

这个项目实现了在 CH32V003 微控制器上运行 Linux 操作系统。它通过使用一个 8MB 的 SPI PSRAM 芯片和一个 RISC-V 模拟器(mini-rv32ima)来实现这一点。模拟器是必需的，因为 PSRAM 不能映射到微控制器的地址空间。Linux 内核和 rootfs 在引导时从 SD 卡加载到 PSRAM 中，文件系统基于 FatFs 库。

 * 项目地址：https://github.com/tvlad1234/linux-ch32v003

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-106/.PNG)

## 工具类

### <font color="red">1、exe_to_dll - 将EXE转换为DLL的小工具</font>

这个小工具可以转换 EXE，以便它可以像 DLL 一样加载。工具支持 32 位和 64 位 DLL。

 * 工具地址：https://github.com/hasherezade/exe_to_dll

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-106/exe_to_dll.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

