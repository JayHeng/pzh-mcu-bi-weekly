# 痞子衡嵌入式半月刊： 第 46 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 45 期》](https://www.cnblogs.com/henjay724/p/15646901.html)

## 唠两句

下周二是冬至，历史上的今天：1959年12月18日，世界上第一台晶体管计算机 - IBM7090由美国国际商用机器公司制造成功。

本期共收录 2个资讯、3个项目、1个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、首届“滴水湖中国RISC-V产业论坛”开启</font>

首届“滴水湖中国RISC-V产业论坛”近日在上海开启，会议旨在促进中国RISC-V芯片与应用厂商和投资机构的对接，推动国产RISC-V芯片的快速产业化落地和应用创新。

本届会议最大的亮点在于，会议期间将集中发布和推介10款首批国产RISC-V芯片，这些芯片不仅与应用需求紧密结合在一起，同时也代表着中国先进的IC设计水平。

![](http://henjay724.com/image/biweekly20211218/dishuihu_luntan2.PNG)
![](http://henjay724.com/image/biweekly20211218/dishuihu_luntan.PNG)

### <font color="red">2、2021 RT-Thread开发者大会召开</font>

2021 RDC (RT-Thread Developer Conference,RT-Thread 开发者大会)以“Beyond”为主题，寓意超越自我，突破边界，RT-Thread将展示其最新的技术动态，产业服务能力。

本届会议四个分会场关于嵌入式的 16 个主题演讲干货满满，还搭配了相应动手环节，绝对的技术盛宴。

![](http://henjay724.com/image/biweekly20211218/2021_RTT_RDC.PNG)
![](http://henjay724.com/image/biweekly20211218/2021_RTT_RDC1.PNG)

## 项目类

### <font color="red">1、PikaScript - 面向嵌入式的超轻量级python引擎</font>

PikaScript（前称mimiscript）是一个完全重写的超轻量级python引擎，零依赖，零配置，可以在少于4KB的RAM下运行(如stm32g030c8和stm32f103c8)，极易部署和扩展。

> 项目地址：https://github.com/pikasTech/pikascript

PikaScript是使用c语言写成的开源脚本支持库，可以非侵入地为mcu提供面向对象的脚本支持。PikaScript能够将c语言的原生函数以及变量绑定到脚本对象上，然后直接使用脚本调用。其架构图如下：

![](http://henjay724.com/image/biweekly20211218/mimiScript.PNG)

### <font color="red">2、Ring-Buffer - 仅80行代码的超简洁环形队列</font>

Ring-Buffer 是特意为嵌入式系统精简优化的环形队列，源代码仅 80 行，实现简洁可靠。

> 项目地址：https://github.com/AndersKaloer/Ring-Buffer

### <font color="red">3、ATmega-Soldering-Station - 成熟的 T12 焊台控制器</font>

这个项目包含了开发 T12 焊台所需的全部软硬件设计，PID 参数都是成熟的，功能完成度非常高。

> 项目地址：https://github.com/wagiminator/ATmega-Soldering-Station

```text
1. 烙铁头温度实时监测
2. PID温度控制
3. 可以通过编码器进行控制温度
4. 短按编码器进入短时升温模式
5. 长按编码器进入主菜单
6. 手柄震动检测（需要手柄含有震动传感器）
7. 手柄连接检测（通过判断烙铁头温度是否能够被读取来实现）
8. 定时器设定 - 随眠，关机时间
9. 可以测量主控芯片电压以及温度
10. 在OLED上实现信息显示
11. 允许设置不同烙铁头的温度校准值
12. 设置被保存在EEPROM，掉电不丢失
13. 允许热插拔烙铁头，并弹出烙铁头配置选择菜单
```

![](http://henjay724.com/image/biweekly20211218/T12_Soldering_Station.PNG)

## i.MXRT出品

### <font color="red">1、北京智慧水务发展研究院 - 边缘抄表器</font>

这是一个由北京智慧水务发展研究院和北京鸿成鑫鼎智能科技有限公司联合开发的“边缘抄表器”模块，这个模块将率先用于机械水表的智能抄表。这个边缘智能抄表模块采用恩智浦i.MXRT1020跨界单片机读取摄像头并运行基于深度学习的“SlimSSD”检测算法，直接扣在水表表盘上就可以拍照并且识别表盘的读数。

> * RT芯片：i.MXRT1021
> * 产品主页： N/A
> * 官网定价： N/A

![](http://henjay724.com/image/biweekly20211218/AI_ChaoBiao_1020.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

