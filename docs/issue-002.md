# 痞子衡嵌入式半月刊： 第 2 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 1 期》](https://www.cnblogs.com/henjay724/p/12285491.html)

## 唠两句

今天是立春与雨水交节，雨水节气标示着降雨开始、雨量渐增，俗话说“春雨贵如油”，适宜的降水对农作物的生长很重要。

受疫情影响，相信本周大部分朋友还是 Work at home 居多，在家里办公效率肯定不如在公司，不过如果能借此机会潜心下来阅读技术文档或者写一些工作小结，或许能更有收获。

从本期开始，增加《i.MXRT出品》分类，推介基于i.MXRT系列的客户产品。

本期共收录 1条资讯、4个项目、2个工具、2个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、ARM 发布面向 AI/ML 的 Cortex-M55 内核以及 Ethos-U55 microNPU</font>

ARM 近日公布了最新 Cortex-M 系列内核(Cortex-M55)，还同时推出了 Ethos-U55 microNPU，旨在为低功耗嵌入式设备提升机器学习和推理能力，扩展产品组合以满足新的需求。

Cortex-M55 与 Ethos-U55 结合使用，能巨大的提升性能，与前几代 Cortex-M 芯片相比，总的处理能力能提高 480 倍。

关于这两个新品的更多细节，详见痞子衡的这两篇小文：[《单片机AI的春天已来，ARM Cortex-M55发布了》](https://www.cnblogs.com/henjay724/p/12293565.html)、[《Ethos-U55，ARM首款面向Cortex-M的microNPU》](https://www.cnblogs.com/henjay724/p/12312210.html)。

![](http://henjay724.com/image/biweekly/Cortex-M55_Ethos-U55.JPG)

## 项目类

### <font color="red">1、JuulLabs-OSS/mcuboot - 适用于 32-bit MCU 的通用安全 Bootloader</font>

mcuboot 是由 JuulLabs-OSS 组织维护的开源 Bootloader 项目，它可以让你轻松实现 MCU 应用程序安全升级。

> 项目主页： https://mcuboot.com/

这个 Bootloader 适用于 32-bit MCU，其跟具体 MCU 硬件平台无关，它目前已经适配了 Zephyr 和 Mynewt 两款操作系统，当然如果手工移植 MCU 硬件驱动，其也可以跑在裸机上。

用户程序仅支持 AES-CTR-128 加解密（纯软件实现），有专门配套 imgtool 脚本来完成程序加密，密钥本身支持加密的算法选择较多，包含 RSA-OAEP、AES-KW-128、ECIES-P256。

恩智浦 AE 团队做的 i.MXRT OTA 方案中就使用了 mcuboot 来实现应用程序升级。

![](http://henjay724.com/image/biweekly/imxrt_ota_framework.JPG)

### <font color="red">2、BalanceCar - 基于恩智浦 MKE18F 的蓝牙控制两轮自平衡小车</font>

这是恩智浦 GCC 俱乐部发起的一个两轮自平衡小车 DIY 项目，硬件原理图、源代码全部开源。

> 项目主页：https://gitee.com/suyong_yq/BalanceCar

![](http://henjay724.com/image/biweekly/GCC_BalanceCar_m.jpg)

小车主控是恩智浦 MKE18F 系列 MCU，自平衡功能是利用了九轴传感器 MPU9250（3 轴陀螺仪、3 轴加速度计和 3 轴磁力计），传感器数据通过 SPI 接口发送给 MCU 处理。

小车可由蓝牙控制，蓝牙模块可选两种：基于恩智浦 KW41Z 的全功能 BLE 模块或者信泰微 JDY-10 BLE4.0 从机模块。

应用端兼容 "平衡小车之家(http://www.minibalance.com/)" 提供的 Mini Balance App 应用程序（Android 4.4 系统及更高版本）。

![](http://henjay724.com/image/biweekly/MiniBalance_App.JPG)

### <font color="red">3、Avem - 基于意法半导体 STM32F103 的轻量级无人机飞控</font>

这是 "我爱模型(http://bbs.5imx.com/)" 网友 but1n 搞的一个轻量级无人机飞控，除了必备的飞行姿态控制之外，还计划实现超视距飞行。

> 项目主页：https://github.com/avem-labs/Avem

![](http://henjay724.com/image/biweekly/Avem_product.JPG)

无人机主控是意法半导体 STM32F103 系列 MCU，飞控功能是利用了六轴传感器 MPU6050（3 轴陀螺仪和 3 轴加速度计），传感器数据通过 I2C 接口发送给 MCU 处理，姿态控制算法是该网友自己写的所谓串级 PID。无人机可搭配 GPS 模块来实现超视距飞行。

![](http://henjay724.com/image/biweekly/Avem_framework.JPG)

### <font color="red">4、myPhone - 基于微芯 ATmega128 的简易 GSM 手机原型</font>

这是一位瑞士小伙 Akos Pasztor 搞的一个简易 GSM 手机原型，可连接 GSM 网络拨打和接听电话。

> 项目主页：https://akospasztor.com/projects/myphone-v2/

这个手机原型主控是 ATmega128，网络功能则是基于 HUAWEI EM310 GSM 模块，显示部分用的一个 4x16 字符型 LCD（显示号码，网络服务商，信号强度等），其内部还有一颗 512Kbit SPI EEPROM 来实现联络人的存储。

这个原型共有两版，v1 版需要外部供电且键盘在主 PCB 上，v2 版增加了电池供电并且使用了薄膜按键。

![](http://henjay724.com/image/biweekly/myPhone.JPG)

## 工具类

### <font color="red">1、Sublime Text - 最受程序员喜爱的代码编辑器</font>

Sublime Text 是一个具有代码高亮、语法提示、格式化，自动补齐且反应极快的编辑器，不仅具有华丽的界面，还支持插件扩展机制，用它来写代码，绝对是一种享受。

> 工具主页： http://www.sublimetext.com/

于嵌入式开发人员而言，除 IDE 外，大部分人的专用编辑器启蒙老师应该是 Source Insight，不过 Source Insight 是强制要 license 的，所以不妨试一下 Sublime Text，痞子衡的同事几乎都在用它。

编辑器千千万，为什么单独推荐它？不为别的，这是唯一一个用性感来形容的编辑器，自己去体验吧。

![](http://henjay724.com/image/biweekly/SublimeText_440x336.gif)

### <font color="red">2、ADALM2000 - 亚德诺(ADI)半导体出品的11种功能合一的便携口袋仪器</font>

ADALM2000 是由业界卓越的半导体公司 ADI 面向电子相关专业大学生和爱好者推出的一款便携式、多功能测试测量仪器。

> 产品主页： https://www.analog.com/cn/design-center/evaluation-hardware-and-software/evaluation-boards-kits/ADALM2000.html

上一期痞子衡推荐过以意法半导体 STM32H750 系列为主芯片的多功能仪器 H7-TOOL，充分利用了 MCU 片内 ADC/DAC，它的特点在于源代码全开源，可玩性强。而 ADALM2000 主处理芯片是采用赛灵思的Zynq-7010系列SoC，配合 ADI 自家的高性能 ADC/DAC，它是一款商业级口袋仪器。

H7-TOOL 售价是 528 元，ADALM2000 官网标价 $149。

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

## i.MXRT出品

### <font color="red">1、大疆创新 - 机甲大师(RoboMaster) S1</font>

RoboMaster S1 是一款智能教育机器人，以寓教于乐的形式为你开启编程、机器人控制及人工智能相关知识的学习之旅。

> RT芯片：i.MXRT1021
> 产品主页： https://www.dji.com/cn/robomaster-s1
> 官网定价： 3499 元起

![](http://henjay724.com/image/biweekly/RoboMaster_440x246.gif)

### <font color="red">2、大疆创新 - 航拍小飞机(御Mavic Mini)</font>

御Mavic Mini 是一款航拍小飞机，强大飞行性能注入在轻小机身中，助你畅快飞行，随心创作，发现熟悉的事物另一面的美。

> RT芯片：i.MXRT1061
> 产品主页： https://www.dji.com/cn/mavic-mini
> 官网定价： 2699 元起

![](http://henjay724.com/image/biweekly/MavicMin_440x246.gif)
