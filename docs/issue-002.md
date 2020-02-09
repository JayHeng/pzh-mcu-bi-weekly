# 痞子衡嵌入式半月刊： 第 2 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

## 唠两句


本期共收录 x条资讯、x个项目、x个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、</font>

![]()



## 项目类

### <font color="red">1、</font>


## 工具类

### <font color="red">1、ADALM2000 - 亚德诺(ADI)半导体出品的11种功能合一的便携口袋仪器</font>

ADALM2000 是由业界卓越的半导体公司 ADI 面向电子相关专业大学生和爱好者推出的一款便携式、多功能测试测量仪器。

上一期痞子衡给大家推荐过安富莱出品的以意法半导体 STM32H750 系列为主芯片的多功能仪器 H7-TOOL，充分利用了 MCU 片内 ADC/DAC，它的特点在于源代码全开源，可玩性强。而 ADALM2000 主处理芯片是采用赛灵思的Zynq-7010系列SoC，配合 ADI 自家的高性能 ADC/DAC，它是一款商业级口袋仪器。

H7-TOOL 售价是 528 元，ADALM2000 官网标价 $149。

> 产品主页： https://www.analog.com/cn/design-center/evaluation-hardware-and-software/evaluation-boards-kits/ADALM2000.html

![](http://henjay724.com/image/biweekly/ADALM2000-web.png)

ADALM2000 的主要功能点如下：

```text
1、双通道USB数字示波器 - 100Msps 12位ADC
2、双通道任意函数发生器 - 150Msps 12位DAC
3、16通道数字逻辑分析仪（兼容3.3V CMOS和1.8V或5V，100MS/s）
4、16通道模式发生器（3.3V CMOS，100MS/s）
5、16通道虚拟数字I/O
6、用于链接多个仪器的两个输入/输出数字触发信号(3.3V CMOS)
7、单通道电压表（AC、DC、±20V）
8、网络分析仪 – 电路波特、奈奎斯特、尼克尔斯传输图。范围：1Hz至10MHz
9、频谱分析仪 – 功率频谱和频谱测量（噪底、SFDR、SNR、THD等）
10、数字总线分析仪（SPI、I²C、UART、并行）
11、两个可编程电源（0…+5V、0…-5V）
```

ADALM2000 固件并没有开源，但配套上位机 Scopy 是开源的，Scopy 提供了直观的用户图形界面，即便是第一次使用，上手也是非常简单的。

> 开源上位机： https://github.com/analogdevicesinc/scopy

![](http://henjay724.com/image/biweekly/Scopy.jpg)