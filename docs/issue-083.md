# 痞子衡嵌入式半月刊： 第 83 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 82 期》](https://www.cnblogs.com/henjay724/p/17744244.html)

## 唠两句

历史上的今天：1938年10月22日，美国物理学家卡尔森发明印刷史上的重大突破 - 静电复印技术。

本期共收录 1 个资讯、2 个项目、2 个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、兆易创新推出GD32VW553系列全新Wi-Fi 6 MCU</font>

近日兆易创新GigaDevice宣布正式推出基于 RISC-V 内核的 GD32VW553 系列双模无线微控制器。

GD32VW553 系列 MCU 集成的2.4GHz Wi-Fi 6射频模块采用IEEE 802.11ax标准，并向下兼容IEEE 802.11b/g/n标准，可以适用于不同的网络环境。支持正交频分多址(OFDMA)，实现多部设备共享信道资源，数据传输速率相比Wi-Fi 4提高了60%;还支持多用户多输入多输出(MU-MIMO)，能协同多部设备同时工作且互不干扰。从而在多设备高密度接入场景下实现高效率低延迟通信。

GD32VW553 系列 MCU 片上集成的Bluetooth LE 5.2射频模块，能够以最新的蓝牙规范延长通信距离、提高吞吐量、增强安全性和节省电能。提供了2Mbps高速数据模式和125K/500Kbps多种速率，有效缩短传输时间并提高灵敏度。还可以在众多设备及复杂环境下协助组建及配置起稳定快速的无线网络。

> * 资讯来源：https://www.gd32mcu.com/cn/detail/532

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-083/GD32VW553.png)

## 项目类

### <font color="red">1、ATtiny412-USB-Power-Isolator - 低成本2.5KV USB电源隔离方案</font>

对于某些应用，需要电隔离电源以避免接地回路或短路，或仅仅是为了相互保护。ATtiny412-USB-Power-Isolator 提供了USB电源适配器的5V轨道的简单隔离(2.5kV)的可能性，输出不稳定，最大连续电流为1A。需要注意的是本项目仅隔离电源轨，要完全隔离包括数据线，请查看作者的另一个项目 ADuM3160-USB-Isolator。

> * 项目地址：https://github.com/wagiminator/ATtiny412-USB-Power-Isolator

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-083/ATtiny412-USB-Power-Isolator1.PNG)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-083/ATtiny412-USB-Power-Isolator2.PNG)

### <font color="red">2、The-Open-Book - 软硬件全开源的电子书阅读器</font>

Open Book 是国外工程师 Joey 长期以来尝试设计的一款易于理解和使用的电子书阅读器。目前的版本是“精简版”或“开发者预览版”。它的设计非常简单: 有7个通孔和14个表面贴装组件，几乎全部在一个厚实的1206封装，很容易手工焊接。缺点是它没有LiPo充电电路; 相反，它使用AAA电池，使它比以前的版本更笨重。Open Book 软硬件是全开源的。

> * 项目地址：https://github.com/joeycastillo/The-Open-Book

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-083/The-Open-Book1.PNG)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-083/The-Open-Book2.PNG)

## 工具类

### <font color="red">1、KiKit - KiCAD开源拼板助手</font>

KiKit 是一个 Python 库，KiCAD 插件和 CLI 工具，用于自动执行标准 KiCAD 工作流中的若干任务，如:

```text
- 按特定规则和奇怪的形状嵌板
- 根据制造商预设自动导出制造数据
- KiCAD 多板项目
- 创建板卡演示页面
```

> * 工具地址：https://github.com/yaqwsx/KiKit

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-083/KiKit.jpg)

### <font color="red">2、StateSmith - 开源状态机代码生成工具</font>

StateSmith 是一个跨平台、免费/开源的工具，用于用多种编程语言生成状态机。生成的代码可读性高，具有零依赖关系，适用于微型裸机微控制器，视频游戏，应用程序，网络，计算机…

> * 工具地址：https://github.com/StateSmith/StateSmith

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-083/StateSmith.png)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

