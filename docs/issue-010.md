# 痞子衡嵌入式半月刊： 第 10 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 9 期》](https://www.cnblogs.com/henjay724/p/13050513.html)

## 唠两句


本期共收录 x条资讯、x个项目、x个工具、x个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、低功耗，多协议，内置NFC选件：恩智浦推出K32W061/41</font>

恩智浦半导体近日宣布推出新的超低功耗、多协议无线微控制器（MCU）系列K32W061/41。新的低功耗设备完善了NXP近期推出的引脚兼容JN5189/88（Thread / Zigbee）和QN9090/30（Bluetooth LE）MCU，为原始设备制造商（OEM）带来更轻松的迁移路径，帮助他们支持现有和新兴的智能家居，构建使用案例。

> 芯片主页: https://www.nxp.com.cn/products/wireless/thread/k32w061-41-high-performance-secure-and-ultra-low-power-mcu-for-zigbeethread-and-bluetooth-le-5-0-with-built-in-nfc-option:K32W061_41?cid=wechat_iot_005321

![](http://henjay724.com/image/biweekly/NXP_K32W0x1.png)

K32W061和K32W041采用IEEE 802.15.4无线电，支持Thread和Zigbee网络协议、蓝牙低能耗5.0和集成式NFC NTAG（K32W061）。该设备还支持较宽工作温度范围（-40℃至+125℃）。作为Zigbee联盟和Thread Group的创始成员之一、NFC Forum联合创始人和Bluetooth SIG成员，恩智浦充分利用无线专业知识以及广泛的MCU能力，集成最新连接标准和适当的智能外设。这些外设支持各种使用案例，包括：

```text
1. 家庭与楼宇自动化
2. 保安和门禁控制
3. 智能恒温器和门锁
4. 网关和传感器网络应用
```

### <font color="red">2、强强联合, 乐鑫发布与百度联名AIoT语音模组及开发板</font>

近日，乐鑫发布了与百度联名的AIoT语音模组ESP32-DU1906及开发板ESP32-Korvo-DU1906，为用户提供集Wi-Fi、经典蓝牙、低功耗蓝牙以及语音处理功能为一体的 AIoT 语音方案，将给用户带来领先的唤醒效果和智能语音交互体验。 

> 开发板主页: https://www.espressif.com/zh-hans/products/devkits/esp32-korvo-du1906

ESP32-DU1906语音模组搭载乐鑫ESP32-D0WD-V3 芯片和百度鸿鹄语音芯片DU1906，具备行业领先的技术规格。ESP32-Korvo-DU1906开发板基于ESP32-DU1906模组设计，能够提供先进的端到端语音解决方案，具有高效率的一体化 AI 服务能力，同时提供端云一体的设备级 AIoT 平台，大大降低了物联网 AI 接入门槛。 

![](http://henjay724.com/image/biweekly/ESP32-Korvo-DU1906.png)

ESP32-Korvo-DU1906方案适用场景十分广泛。它不仅支持 Wi-Fi、Bluetooth、Bluetooth LE、Mesh 等多种无线通讯协议，还支持多类主流音频格式播放以及蓝牙音箱功能。同时，它具备丰富的外设接口，方便连接各类 AIoT 应用产品，能在智能家居（音箱、冰箱、空调等多种家居场景）、智能物联（智能办公、智能支付、智能机器人等）等语音交互场景中实现出色的语音控制，给用户带来全新的智能体验。

### <font color="red">3、恩智浦针对汽车和工业市场推出强化蓝牙功能的KW37/8/9</font>

近日，全球领先的半导体供应商NXP宣布KW3x系列MCU推出新产品KW39/38/37。KW39/38/37增加了对蓝牙5.0长距离传输和蓝牙广告信道扩展等功能。在支持低功耗蓝牙5.0全部新功能的同时，实现与前代产品KW34/35/36在硬件、软件和工具兼容性方面的无缝迁移。

> 芯片主页: https://www.nxp.com.cn/products/wireless/bluetooth-low-energy/kw39-38-37-32-bit-bluetooth-5-0-long-range-mcus-with-can-fd-and-lin-bus-options-arm-cortex-m0-plus-core:KW39-38-37

产品特点：

```text
- 高达48MHz Arm Cortex-M0+内核
- KW37：512KB可编程闪存，带ECC功能; 
- KW39/38：
	256KB可编程闪存 + 256KB FlexNVM，带ECC功能
	8KB FlexRAM支持EEPROM仿真
- 片上64KB SRAM
- 2.4 GHz低功耗蓝牙(BLE) 5.0无线电在任何主/从组合中最多支持8个并发安全连接
- 在BLE 1Mbps模式下提供-98 dBm接收机灵敏度，在BLE远程125kbps模式下提供-105 dBm接收灵敏度
- 增强型BLE自动深度睡眠模式(DSM)支持从设备延迟
- 低功耗模式(VLLS0)电流：250 nA
- AEC Q100 2级汽车认证(KW39A/38A/37A)，工业认证资格(KW38Z/37Z)
- AES-128硬件加速器(AESA)，带LTC；真随机数生成器(TRNG)；每个芯片具有80位唯一识别号；40位唯一介质访问控制(MAC)子地址；LE安全连接
```

![](http://henjay724.com/image/biweekly/KW39-38-37-BD.png)

该产品组合与EdgeVerse平台的处理能力相结合后，恩智浦能够支持智能互联设备，使生活更轻松、更安全、更便捷。该系列芯片非常适合汽车行业的应用，例如无钥匙进入、传感器和无线车载诊断功能。此外，还能实现多种工业应用，例如楼宇控制和监控、防火和安全、家庭和机构医疗、资产管理和监控以及各种其他工业应用。 

## 项目类

### <font color="red">1、TinyGSM - 用于GSM模块的小型Arduino库</font>

TinyGSM是一个由网友vshymanskyy维护的小型的用于GSM模块的Arduino库。该库可以容易的集成到使用Ethernet或WiFi的项目中去，并且项目中已经提供了**PubSubClient (MQTT)**, **Blynk**, **HTTP Client** 以及 **File Download**等示例程序。  

> 项目主页: https://github.com/vshymanskyy/TinyGSM 

该库目前支持的板卡/模块有：

```text
- Arduino MKR GSM 1400
- GPRSbee
- Microduino GSM
- Adafruit FONA (Mini Cellular GSM Breakout)
- Adafruit FONA 800/808 Shield
- Industruino GSM
- RAK WisLTE (alpha)
```

![](http://henjay724.com/image/biweekly/TinyGSM.png)

该项目的完整的WebClient的示例在Arduino Uno上运行仅使用了46%的Flash空间及28%的RAM空间，均小于Arduino GSM库的49%及54%。感兴趣的开发者可以使用这个库到自己的项目中以匀出更多空间用于自己的应用。


## 工具类



## i.MXRT出品




