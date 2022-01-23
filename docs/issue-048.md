# 痞子衡嵌入式半月刊： 第 48 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 47 期》](https://www.cnblogs.com/henjay724/p/15782144.html)

## 唠两句

本周四是大寒，历史上的今天：2004年1月23日，在环火星轨道上运行的欧洲航天局“火星快车”探测器在火星表面发现了水的痕迹，这是人类首次在火星表面发现水。

本期共收录 2个资讯、2个项目、1个工具、2个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、灵动微电子加推基于STAR-MC1内核的微控制器MM32F5270</font>

MM32F5270 是灵动第一款搭载了安谋科技 Arm China STAR-MC1 内核的 MCU 产品，其工作频率可达 120MHz，内置多达 2.25MB Flash 和 192KB RAM，配置FPU、DSP、信号间互联矩阵 MindSwitch、可配置逻辑单元 CLU、三角函数加速单元 CORDIC等算法加速单元，并集成了丰富的外设模块和充足的 I/O 端口。

> * 产品主页：https://www.mindmotion.com.cn/products/mm32mcu/mm32f/mm32f_performance/mm32f5270/

MM32F5270 相较于灵动现有产品全面提升了性能、存储容量、总线架构和外设配置，旨在覆盖更广泛的工业、汽车和 IoT 应用。

![](http://henjay724.com/image/biweekly20220123/MM32F5270.PNG)

### <font color="red">2、云途半导体首款微控制器YTM32B1L通过AEC-Q100车规认证</font>

YTM32B1L系列产品是云途半导体2021年初推出的首款车规级32位MCU芯片，主要应用于传感器控制、胎压监测、座椅、电动尾门、车窗以及车灯控制等应用。

近日、云途宣布YTM32B1L系列产品成功通过AEC-Q100车规认证，其中包括加速环境应力可靠性检验、加速寿命模拟可靠性验证、封装可靠性检验、芯片晶圆制程可靠性检验、电学参数验证、缺陷筛选检验等最高 28 项车规芯片认证。

> * 资讯来源：https://mp.weixin.qq.com/s?src=11&timestamp=1642928090&ver=3575&signature=4cyVmwbdLExyWsPMjGmxds2FeXWHOK-xbmR4i-tf8KPhTi5N-Y9mvp3qJCVd3lFj01EAkXsUGJdWB4E05pf-DXuSJy8U9nSXa*164RjvQaWOtsOMQWC4TuksJOEOIBTK&new=1

![](http://henjay724.com/image/biweekly20220123/YTM32B1L.PNG)

## 项目类

### <font color="red">1、串口U盘 - 基于STM32+CH375的郁闷的工程师利器</font>

辛勤地打工的工程师们，你们是否曾经有过这样的经历,自己辛辛苦苦为公司写的代码和设计的PCB，却无论如何都不能据为己有？因为公司不允许个人电脑上网，因为公司的电脑居然把USB口也封闭了！这时候，我们是万般地郁闷，但是，作为一个以电子开发为主的公司，无论他把多少个USB口封了，都永远会留给你一个串口！

正是这个串口，使我们想到了这样的一个东西 - 串口也可插U盘，设计思路：利用STM32的ARM CPU作为主控+CH375 USB HOST芯片，设计出一个转换板，U盘插进这个板上，板的另一头则是串口，插到电脑上，利用常用的串口调试工具SSCOM或者WINDOW的超级终端，实现把电脑上任意文件通过232传送到U盘上。

> * 项目来源：https://www.amobbs.com/thread-3339369-1-12.html

![](http://henjay724.com/image/biweekly20220123/STM32+CH375_USB_UART.PNG)

### <font color="red">2、Arduino Laser Infrared Thermometer - 基于 Arduino 的便携式红外测温仪</font>

红外测温仪能够测量物体的表面温度，其优点是非接触式测温，可以方便且精准地测量远端物体温度，应用广泛。这个项目包括自制一把红外测温仪所需要的材料、工具和制造的方法等全部流程。

> * 项目主页1：https://make.quwj.com/project/157
> * 项目主页2：https://www.instructables.com/Arduino-Laser-Infrared-Thermometer/

这个项目使用的是 GY-906 红外线温度计传感器。这款模块非常便宜，易于集成，并且支持带有 10K 上拉电阻的 I2C 接口 。此款温度传感器的出厂校准为：传感器温度范围为 -40 至 125 摄氏度，物体温度范围为 -70 至 380 摄氏度。传感器的误差范围约为 0.5 摄氏度。

![](http://henjay724.com/image/biweekly20220123/Arduino_Laser_Infrared_Thermometer.PNG)

## 工具类

### <font color="red">1、WOKWI - 在线的Arduino/ESP32/树莓派Pico仿真学习平台</font>

WOKWI 是一个很酷的支持Arduino、ESP32、树莓派Pico在线仿真学习的网站。

> * 软件官网：https://wokwi.com/

WOKWI 网站特点如下：

```text
1. 完全免费
2. 基于浏览器（无需安装，无需下载！）
3. 支持多种板卡（UNO、Mega、Nano、ATtiny85、Franzzininho、Raspberry Pi Pico 等）
4. 易于与他人共享项目（它只是一个链接，任何人都可以从其他位置打开项目）
5. 支持多种传感器 - 湿度传感器、模拟和数字温度传感器、PIR传感器、运动传感器等
6. 多种显示器 - OLED、LCD、数码管、智能LED等
```

![](http://henjay724.com/image/biweekly20220123/WOKWI2.PNG)

## i.MXRT出品

### <font color="red">1、大疆创新 - 无线麦克风(Mic)</font>

DJI Mic 是一款紧凑轻巧、性能强大的无线收音系统，由一个双通道接收器和两个无线发射器组成，可实现远达 250 米无线收音距离。两个发射器能同时录音，无论人声、环境声、乐器声，均可清晰录制。两个发射器均自带内置存储，可单独用作录音笔，也可在录音时备份声音，保障录音数据完整性。

> * RT芯片：i.MXRT685
> * 产品主页： https://www.dji.com/cn/mic
> * 官网定价： 2299 元起

![](http://henjay724.com/image/biweekly20220123/DJI-MIC.PNG)

### <font color="red">2、野火电子 - fireFlasher Mini脱机下载器</font>

fireFlasher MINI 是野火科技推出的脱机烧录器，可以在脱离电脑端的情况下对芯片进行脱机烧录。它支持使用 SWD 接口烧录程序到开发板，可以将多个固件一次烧录到开发板中。

> * RT芯片：i.MXRT1011
> * 产品主页： https://doc.embedfire.com/products/link/zh/latest/tool/fireFlasher-mini/fireFlasher-mini.html
> * 官网定价： 198 元

![](http://henjay724.com/image/biweekly20220123/fireFlasherMini_view.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

