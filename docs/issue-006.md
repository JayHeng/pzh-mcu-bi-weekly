# 痞子衡嵌入式半月刊： 第 6 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 5 期》](https://www.cnblogs.com/henjay724/p/12633951.html)

## 唠两句

今天是谷雨，春季的最后一个节气。

本期共收录 2条资讯、3个项目、1个工具、1个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、</font>


### <font color="red">2、</font>



## 项目类

### <font color="red">1、u8g2 - 一个用于嵌入式设备的单色 OLED/LCD 图形库</font>

u8g2 是目前 Arduino 平台上使用最广泛的单色图形库。U8g2 支持单色 OLED 和 LCD，基本上主流的显示控制器都支持。

> 项目主页：https://github.com/olikraus/u8g2

为什么要运用 u8g2 库？也就是说 u8g2 库能带给我们什么样的开发便利。主要有以下几点：

```text
- u8g2 库平台支持性好，基本上支持绝大部分 Arduino 开发板；
- u8g2 库显示控制器支持性好，基本上市面上的 OLED 都完美支持；
- u8g2 库 API 众多，特别支持了中文，支持了不同字体，这是一个对于开发者俩说不小的福利。
```

这是一张官方提供的 U8G2 库测试图，基于 ESP32 和 SSD1306 OLED：

![](http://henjay724.com/image/biweekly/u8g2_esp32_ssd1306_oled.PNG)

### <font color="red">2、emXGUI - 一个经过十年深度优化的图像引擎(GUI)</font>

emXGUI 是由国内刘巍于 2008 年开始编写，2010 年开始商用的一款图像引擎，主要产品是警用酒精检测仪，产品主要是出口，没有在国内宣传过。

> 项目主页：http://www.emxgui.com/

emXGUI 源码不开源，提供多平台的 LIB 文件，提供完善的 API 手册，无论是个人还是公司都可以很快的上手。目前测试过的平台有：Cortex-M0/3/4/7，Cortex-A系列，ARM9 等。

emXGUI 的特色如下：
```text
1、占用资源少，效率高，在STM32F103不外扩RAM的情况下可以流畅运行
3、友好地支持矢量字体，提供矢量字体制作工具，除了制作矢量字体外，还可以制作矢量的符号
3、使用unicode字符编码支持多国语言，中文，英文，越南语，西班牙语等等
4、支持鼠标，支持触摸
5、自带滑动控件，非常方便，即在液晶屏上可以实现类似现在手机界面滑动的效果
6、高性能的绘图引擎+高效的Z序剪切策略 双管齐下
```

![](http://henjay724.com/image/biweekly/emXGUI_tests.png)

### <font color="red">3、LearningGUI - 一款100%使用 C 语言开发的通用嵌入式开源 GUI</font>

LearningGUI 被设计成独立于具体的硬件平台和具体的软件平台，是一款通用的嵌入式开源 GUI 系统。LearningGUI 的目标是替代 emWin，同时抢占中低端的 QT 市场。

LearningGUI 无浮点运算，只调用 C，无汇编代码。显示，键盘，鼠标等驱动由用户在应用中编写注册，因此，LearningGUI 的通用性,可移植性非常好！它可以裸奔，也可以在 RTOS 上运行，同时更适合在 Linux 下运行。

LearningGUI 的特色如下：
```text
1、占用内存小。Basic版实行静态内存管理，占用10多K RAM. Windows版实行动态内存管理，占用内存与建立控件多少相关。
2、支持内置GB2312—80标准汉字库。
3、提供开放式字库访问接口。
4、提供开放式颜色转换接口。
5、提供消息驱动机制。
6、提供类似于Win32 SDK式样的API接口。
```

![](http://henjay724.com/image/biweekly/LearningGUI_test.jpg)

## 工具类

### <font color="red">1、 </font>



## i.MXRT出品

### <font color="red">1、新北洋 - 针式收据打印机(BTP-M180II)</font>

BTP-M180II 是新北洋推出的升级款针式收据打印机，打印相关部件可靠性全面提升，固件控制更智能，继承了上一代产品更换耗材方便快捷、耗材适应性强等全部优势，稳定性全面提升。

> RT芯片：i.MXRT1050
> 产品主页： http://www.snbc.cn/product/1289.html
> 参考售价： 369 元

![](http://henjay724.com/image/biweekly/SNBC_BTP-M180II.PNG)

