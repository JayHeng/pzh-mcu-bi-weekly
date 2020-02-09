# 痞子衡嵌入式半月刊： 第 1 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

## 唠两句

今天是农历庚子鼠年正月十五，传统元宵佳节，但因为 2019-nCoV 肺炎疫情不减，节日气氛平淡了些。

原计划这个半月刊能按二十四节气交节之日准时发布，但这第一期就没能准时，离立春已经过去4天了，也罢，规矩一开始就破了，底下发布时间压力上也就小了。

大家都知道痞子衡东家是飞思卡尔/恩智浦半导体，所以这第一期咱偏袒一下东家，多给恩智浦相关产品一些特写。

本期共收录 3条资讯、3个项目、2个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、划时代 1GHz 主频 MCU 恩智浦 i.MXRT1170 有望 2020 年下半年面市</font>

2019年10月2日恩智浦半导体隆重发布了 i.MXRT1170，这是一款划时代的 MCU。因为它，单片机首次迈入 1GHz 主频大关，这对于嵌入式从业人员来说，是个值得铭记的时刻。

这款性能炸裂的 MCU 大家都非常期待，在各大嵌入式技术交流群里，它也被频繁提及和讨论，它什么时候能供货是大家最关心的问题。据目前进展来看，i.MXRT1170 有望今年下半年开始供货，所谓好货不怕晚，它绝对值得等待。还有大家比较关心的价格，i.MXRT1170 其实会是一个系列(从 RT1171 到 RT1176 )的方式推出，预计入门级起价在 5$ 的样子。

让我们再来回顾一下 i.MXRT1170 的厉害之处。i.MX RT系列从 RT1170 开始首次引入了双核，Cortex-M4 的引入可不仅仅是刷新 CoreMark 总分那么简单（当然6468的跑分确实挺震撼），有了这颗 Cortex-M4，一些相对简单的键盘响应、传感器采集、电机控制等任务便可以交给它来做，而超强的 Cortex-M7 则可以专注在音视频识别与处理、千兆以太网通讯控制等复杂任务上。

![](http://henjay724.com/image/biweekly/i.MX-RT1170-DualCore-Task.PNG)

更多 i.MXRT1170 的细节，详见痞子衡之前写的 [《终于可以放开聊一聊i.MXRT1170这颗划时代MCU了》](https://www.cnblogs.com/henjay724/p/11624973.html)。

### <font color="red">2、硬禾学堂正在推出高质量技术直播视频，其中"半导体产业前沿技术讲座"栏目将会有 100 期</font>

鼠年春节假期，电子行业前辈苏公雨老师可没闲着，他创办的专注于“实战技能培训”的“硬禾学堂”在1月30日启动了第一场在线技术直播。

这个技术盛宴现在正以每天3-4场、每场平均两个小时的节奏为全国的电子技术爱好者、工程师、高校师生等提供着高效、高质量技术学习的渠道。

更有来自英国、美国和法国的多位资深工程师受邀为大家奉上更精彩的前沿技术讲座；NXP（是的，痞子衡的两位大牛同事已经分享过人工智能方面的经验）、Lattice、Cypress、ADI的市场和AE团队也已经向全国的工程师朋友分享过了他们的技术、产品和个人成长心得。

> 视频直播/回看入口： https://class.eetree.cn/index

![](http://henjay724.com/image/biweekly/eetree_tech_class.jpg)

硬禾学堂计划在2月17 - 5月31日之间开设 100 期”半导体产业前沿技术大讲堂”的栏目，帮助半导体行业的朋友们以技术直播、系列讲座、短平快教程的方式高效、快速地开展线上市场营销业务，硬禾学堂会提供全方位的平台支撑和宣传推广服务。

### <font color="red">3、翼辉全新设计了一款面向未来物联网需求的新一代小型操作系统 MS-RTOS</font>

2019年11月26日翼辉信息（就是推出知名大型操作系统 SylixOS 的公司）发布了一款面向未来物联网需求的新一代小型操作系统，即 MS-RTOS，这是一个商业级的 RTOS。

> MS-RTOS主页： http://www.acoinfo.com/html/product_list/product16.html

MS-RTOS 最大的特点是开创性地在没有 MMU 和资源极其稀少的 MCU（如Cortex-M3）上也能支持多进程与动态装载技术，使得应用与系统能分离开发、独立升级。

MS-RTOS 支持内核空间内存保护（应用程序通过 syscall 访问内核），使得内核有着非常高的安全性。MS-RTOS 在提供足够丰富功能的同时，保持了高效简洁的实现，对 ROM、RAM 消耗极低，特别适用于对硬件成本敏感、安全性要求特别高的产品。

![](http://henjay724.com/image/biweekly/MS-RTOS-arch-diagram.JPG)

## 项目类

### <font color="red">1、OpenMV-RT - 基于恩智浦 i.MXRT 系列的开源机器视觉AI模块</font>

OpenMV-RT 是一款基于恩智浦最近主打的 i.MXRT 超高性能系列 MCU 的视觉模块，模块设计者是恩智浦大牛工程师宋岩（对，就是 ARM Cortex-M3 权威指南中文版作者）。

> 模块源代码: https://github.com/RockySong/micropython-rocky/tree/omv_initial_integrate

这款模块设计得非常简洁，除了 MCU 最小系统之外，仅包含四大部件：640x480 数字摄像头传感器、九轴姿态传感器、串行 SPI Flash （存放代码）、SD 卡槽（文件系统）。模块还提供了标准 OpenMV 接口，可在 OpenMV 项目生态里任意扩展其他功能模块。

大牛宋岩为这个模块编写了很多 AI 方面的应用实例，如人脸识别、物体识别、性别识别等，这些实例还在持续增长中，所以这可不是一个简单的硬件模块，而是你入门 AI 的极佳机会。

![](http://henjay724.com/image/biweekly/OpenMV-RT-1060.JPG)

更多 OpenMV-RT 的特点，可参看作者写的文章 [《基于i.MX RT1060的可编程视觉模块》](https://mp.weixin.qq.com/s/JkB6K0IcMDRzcHINopxLyA) 和我写的上手实践 [《OpenMV-RT模块初体验》](https://www.cnblogs.com/henjay724/p/11965518.html)。

### <font color="red">2、TheAlgorithms/C - 各种基础算法、数据结构的 C 语言实现</font>

知名开源组织 TheAlgorithms 维护的 C 语言实现的各种基础算法、数据结构示例。所有算法列表详见 [DIRECTORY.md](https://github.com/TheAlgorithms/C/blob/master/DIRECTORY.md)。

> 项目地址： https://github.com/TheAlgorithms/C

有人说，程序其实就是数据结构和算法的集合。只要一个人精通数据结构和算法，那这个人必然也是编程大牛。

这个项目基本涵盖了常见数据结构和算法，而且代码非常简洁，一点都不晦涩，全部理解并手敲一遍，必然让你编程技巧更上一层楼。

![](http://henjay724.com/image/biweekly/TheAlgorithms_lang_list.JPG)

### <font color="red">3、armink/SFUD -  一款基于JEDEC SFDP标准的串行 (SPI) Flash 通用驱动库</font>

SFUD 是一款开源的串行 SPI Flash 通用驱动库，作者是上海睿赛德(RT-Thread)公司技术总监朱天龙大神。

> 项目地址： https://github.com/armink/SFUD

由于现有市面的串行 Flash 种类居多，各个 Flash 的规格及命令存在差异， SFUD 就是为了解决这些 Flash 的差异现状而设计，让我们的产品能够支持不同品牌及规格的 Flash，提高了涉及到 Flash 功能的软件的可重用性及可扩展性，同时也可以规避 Flash 缺货或停产给产品所带来的风险。

SFUD 主要特点是支持 SPI/QSPI 接口、面向对象（同时支持多个 Flash 对象）、可灵活裁剪、扩展性强、支持 4 字节地址。标准资源占用：RAM:0.2KB ROM:5.5KB，最小资源占用：RAM:0.1KB ROM:3.6KB。

SFUD 目前主要提供的 Demo 平台是STM32，但良好的代码结构也很方便移植到其他MCU，下表为所有已在 Demo 平台上进行过真机测试过的 Flash。

![](http://henjay724.com/image/biweekly/SFDP_flash_list.JPG)

## 工具类

### <font color="red">1、MCUXpresso Secure Provisioning Tool v1.0 - 恩智浦官方MCU一站式安全启动/下载工具</font>

恩智浦半导体自 2017 年开始推出 i.MXRT 系列 MCU 以来，让广大嵌入式从业者既爱又恨，爱的是这颗 MCU 的超高性能，恨的是入门较难，配套启动下载工具使用太复杂。如今，千呼万唤的官方一站式启动工具 MCUXpresso Secure Provisioning Tool 终于推出了。

> 工具主页： https://nxp.com/mcuxpresso/secure

使用过 i.MXRT 芯片的朋友应该都知道痞子衡也设计过一个一站式安全启动工具 [NXP-MCUBootUtility](https://github.com/JayHeng/NXP-MCUBootUtility)，代码开源在github上，有近 100 star了，这个工具 2018 年底发布的 v1.0，承担了部分 i.MXRT 客户支持工作。

如今终于等来了官方正式版 MCUXpresso Secure Provisioning Tool，从设计原理上来说，MCUXpresso Secure Provisioning Tool 跟 NXP-MCUBootUtility 其实是类似的，不过 MCUXpresso Secure Provisioning Tool 计划支持所有系统（Windows/Linux/macOS），并且还提供命令行接口，方便自动化测试和批量生产。

![](http://henjay724.com/image/biweekly/MCUXpresso_Secure_Provisioning_Tool.JPG)

MCUXpresso Secure Provisioning Tool v1.0 界面设计得非常清爽，目前仅支持 i.MXRT1050 和 i.MXRT1060，操作上也是足够简单。还不快赶紧下载试用？

![](http://henjay724.com/image/biweekly/MCUXpresso_Secure_Provisioning_Tool_GUI.JPG)

### <font color="red">2、H7-TOOL - 专为单片机工程师设计的一款实用的多功能开发调试工具</font>

H7-TOOL是一个专为单片机工程师设计的实用的多功能开发调试工具，工具作者是安富莱电子大牛硬汉哥，而且原理图和所有代码全部开源。

> 资源汇总贴： http://www.armbbs.cn/forum.php?mod=viewthread&tid=89934

相信很多人有带板子回家调试、或带板子出差调试的情况。因为产品问题是无法预知的，多半情况不可能带齐全套测试工具的。经常遇到手边缺万用表、缺示波器、缺串口线、缺逻辑分析仪而导致工作很难继续。

这时候你就需要一个 H7-TOOL，有了H7-TOOL就等于随时携带了一个小型实验室，各种常用仪器全都齐活了。

![](http://henjay724.com/image/biweekly/H7-TOOL.jpg)

来看看 H7-TOOL 这个“小型实验室”里都有哪些仪器吧，是不是叹为观止？

```text
1、脱机烧录器
2、双通道虚拟示波器（支持以太网和USB两种方式）
3、8 通道逻辑分析仪
4、USB-RS485 转换器
5、USB-RS232 转换器
6、USB-TTL 串口转换器
7、USB-CAN 转换器 (未完成)
8、DAP-Link 仿真器 / 下载器 (未完成)
9、I2C 控制器 (未完成)
10、SPI 控制器 (未完成)
11、GPIO 输入输出控制器
12、信号发生器 & 0-20mA电流输出
13、PWM 发生器 (未完成)
14、脉冲计数器
15、频率计
16、负载电流电压示波器
17、高侧电流表 & 电池放电容量测量
18、双通道电压表
19、电阻测量 通断蜂鸣
20、温度测量
21、二极管测量
22、微型数控电源
```

而且 H7-TOOL 配套上位机工具也非常漂亮易用哦。

![](http://henjay724.com/image/biweekly/H7-TOOL-GUI.png)

