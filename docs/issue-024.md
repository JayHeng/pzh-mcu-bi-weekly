# 痞子衡嵌入式半月刊： 第 24 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 23 期》](https://www.cnblogs.com/henjay724/p/14243692.html)

## 唠两句

这周三是大寒。二十四节气中的最后一个节气，大寒是天气寒冷到极致的意思。

本刊是庚子鼠年最后一刊，很抱歉鸽了4天，最近身边发生了一些重要的事，写文章这块有所暂停。一转眼这个当初只是抱着玩玩的心态搞的嵌入式半月刊已经发了整整24期了，任何一件小事坚持下去都是不容易的。当初夸下海口说至少搞100期，目前完成了1/4，下一个新二十四节气轮回（辛丑牛年），咱们继续再见。

本期共收录 1条资讯、3个项目、1个工具、1个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、树莓派推出首款微控制器级产品Pi Pico</font>

树莓派基金会近日推出了首款微控制器级产品树莓派Pi Pico（Raspberry Pi Pico），这款产品的售价仅为4美元。

> 资讯主页: https://www.raspberrypi.org/blog/raspberry-pi-silicon-pico-now-on-sale/

![](http://henjay724.com/image/biweekly/Raspberry-Pi-Pico.PNG)


树莓派Pi Pico是一款基于树莓派自己设计的全新RP2040芯片打造的开发板，而RP2040微控制器芯片搭载有双核ARM Cortex M0+处理器，运行频率高达133MHz，内置264KB的SRAM，支持多达16MB的片外闪存。

树莓派Pi Pico拥有2MB的闪存，一个单击按钮、一个LED灯和一个Micro USB Type B端口，既小又便宜。它提供了一个灵活的、价格合理的开发平台，可直接部署到终端产品中，从而缩短上市时间。

## 项目类

### <font color="red">1、perf_counter - 专为Cortex-M SysTick设计的性能计数器</font>

perf_counter是ARM公司大神王卓然（江湖绰号傻孩子）维护的项目，是一个Cortex-M SysTick专用的性能计数器。它与用户原有的SysTick功能共享SysTick而不受干扰。这个库将带来新的功能，如time.h中定义的性能计数器、delay_us()和clock()函数。

> 项目主页： https://github.com/GorgonMeducer/perf_counter

### <font color="red">2、microLite - 极简可靠的嵌入式裸机系统软件平台</font>

microLite，是一个嵌入式裸机系统软件平台，基本属性是多个任务顺序执行，本质是前后台系统。经过多年沉淀，microLite功能丰富，性能稳定，可有效降低开发门槛、缩短开发周期。

> 项目介绍： https://blog.csdn.net/xlsbz1/article/details/111655405

![](http://henjay724.com/image/biweekly/microLite.PNG)

microLite作为一个嵌入式裸机系统软件平台，有如下特点：

```text
1. microLite采用C语言编写，与RTOS相比较，其实现更加浅显易懂，模块化编程，方面快速剪裁。
2. 相较于RTOS，microLite体积小、成本低、启动快速，除此之外microLite还具有占用堆栈资源小等特点。
3. microLite集成了文件系统、网络协议栈、驱动框架等，具有丰富的中间件组件。
4. microLite拥有高效、灵活的软件内核定时器API接口。
```

### <font color="red">3、Frequency Probe - 一款超迷你频率探头</font>

国外达人David Johnson设计的超迷你频率探头，这个频率探头能够通过显示频率和电压帮助你调试电路，它能够测出1Hz到5MHz的周期性波形，准确度达到0.3%，当然也可以当电压表使用，能够告诉你当前的电压值。

> 项目主页： http://www.technoblogy.com/show?25C4

![](http://henjay724.com/image/biweekly/FrequencyProbe.PNG)

组装包括：

```text
1. ATtiny84A采用SOIC封装，电阻，电容器和二极管均为0805尺寸，因此手工焊接应相对容易。
2. 晶体为5x3.2mm
3. 显示屏为SSD1306驱动的OLED 128x32 I2C显示模块
4. 用普通的制衣针作为探针
5. 使用了一个40mAh的Lipo电池通过双面自粘泡沫垫固定在板上给板子供电
```


## 工具类

### <font color="red">1、Matlab Simulink - 可用于嵌入式系统的可视化仿真及代码生成工具</font>

Matlab是由MathWorks公司出品的一款数学分析软件，主要用于算法开发，数据分析等领域，而Matlab软件中的一个非常重要组件Simulink，这个组件对于嵌入式开发也能提供很大的帮助。

> 工具主页：https://www.mathworks.com/products/simulink.html?s_tid=hp_products_simulink

Simulink软件可以提供基于事件建模、物理建模、实时仿真与测试、验证与测试以及代码生成的各类工具箱，能满足嵌入式软硬件设计中各阶段的需求。

![](http://henjay724.com/image/biweekly/SImulink_Embedded_coder.png)

## i.MXRT出品

### <font color="red">1、造隆股份 - 摩托车仪表盘VSC-01</font>

造隆摩托车仪表盘VSC-01是一款创新的仪表盘，一改传统摩托车仪表盘的单调设计，功能丰富且酷炫，其GUI采用的是Embedded Wizard。

> * RT芯片：i.MXRT1052   
> * 产品主页： https://www.chaolong.com.tw/en  
> * 官网定价： N/A  

![](http://henjay724.com/image/biweekly/CHAOLONG-VSC-01.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

