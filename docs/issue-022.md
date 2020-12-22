# 痞子衡嵌入式半月刊： 第 22 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 21 期》](https://www.cnblogs.com/henjay724/p/14105847.html)

## 唠两句

昨天是冬至。又称日短至、冬节、亚岁等，兼具自然与人文两大内涵，也是中国民间的传统节日。

本期共收录 0条资讯、2个项目、2个工具、1个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、</font>


## 项目类

### <font color="red">1、LwRB - 一款适用嵌入式系统的轻量级 RingBuffer</font>

ringbuffer（环形缓冲区）可以说是嵌入式应用非常常用的数据缓存设计了，LwRB 是国外开发者 MaJerle 维护实现的轻量级 ringbuffer，是一个为嵌入式系统特殊优化设计的 FIFO。

> 项目主页: https://github.com/MaJerle/lwrb

LwRB 特点：

```text
1. 纯ANSI C99实现, 数据类型兼容于size_t
2. 与具体硬件平台无关
3. 类FIFO缓冲设计
4. 未使用动态内存分配，纯静态内存
5. 特殊优化过的memcpy实现
6. 当用作单写/单读的管道时是线程&中断安全的
7. 适用于DMA在缓冲区和应用程序内存之间进行零拷贝开销的DMA传输
8. 支持数据查看、读跳过、写进
9. 实现对事件通知的支持
```

LwRB 的代码设计很完善了，是个开源项目，更难能可贵的是它的设计文档也相当详实。下图很好地展示了 LwRB 对于不同的缓冲区边界处理情况，可以让你对其内部如何管理数据有个基本理解。

![](http://henjay724.com/image/biweekly/LwRB.PNG)

### <font color="red">2、MultiTimer - 超精简的纯软件定时器驱动</font>

MultiTimer 是网友  0x1abin  开发的一个纯软件定时器扩展模块，可无限扩展你所需的定时器任务，取代传统的标志位判断方式， 更优雅更便捷地管理程序的时间触发时序。

> 项目主页：https://github.com/0x1abin/MultiTimer

MultiTimer 使用用法特别简单：

```C
#include "multi_timer.h"
struct Timer timer;
void timer_callback()
{
    printf("timer timeout!\r\n");
}
int main()
{
    timer_init(&timer, timer_callback, 1000, 1000); //1s loop
    timer_start(&timer);
    while(1)
    {
        timer_loop();
    }
}
void HAL_SYSTICK_Callback(void)
{
    timer_ticks(); //1ms ticks
}
```

## 工具类

### <font color="red">1、DSLogic - 一款跨平台的逻辑信号分析仪</font>

DSLogic是梦源实验室出品的一款基于USB的逻辑分析仪，支持最大采样率高达1GHz，stream模式下最大采样深度16G。DSLogic有配套专用上位机，支持各种模式，例如逻辑分析仪，示波器，数据采集等，随着功能的不断集成和完善，DSLogic被打造成易上手的信号分析综合平台。

> * 产品主页: https://dreamsourcelab.cn/product/dslogic-series/
> * 项目主页: https://github.com/DreamSourceLab/DSLogic-hdl

![](http://henjay724.com/image/biweekly/DreamSourceLab-DSLogic2.PNG)

![](http://henjay724.com/image/biweekly/DreamSourceLab-DSLogic.png)

DSLogic的两大优势：

```text
1.支持Windows / MacOS / Linux。 由于具有开源功能，还可以将DSView移植到个人平台上。
2.易于使用是DreamSourceLab的设计初衷，能够有效、快速地帮助您的项目落地成功。
```

### <font color="red">2、WinHex - 强大的十六进制编辑软件</font>

WinHex是在Windows下运行的十六进制编辑软件，此软件功能非常强大，有完善的分区管理功能和文件管理功能；它能够编辑任何一种文件类型的二进制内容（用十六进制显示）其磁盘编辑器可以编辑物理磁盘或逻辑磁盘的任意扇区。

在嵌入式应用场景下，用它来编辑分析bin文件简单小菜一碟。

> 下载地址： http://www.x-ways.net/winhex/ 

![](http://henjay724.com/image/biweekly/winhex.png)

## i.MXRT出品

### <font color="red">1、格力电器 - 热泵洗护机XQG100</font>

格力热泵洗护机XQG100传承格力空调核心科技，以热泵低温柔烘技术实现衣物烘干，精心细致呵护每件华服。采用自主研发热泵专用双转子变频压缩机，搭载低频转矩控制技术，频率调整更精准，温度控制范围更广，低至37度烘干衣服。

> * RT芯片：i.MXRT1052   
> * 产品主页： https://www.gree.com/cmsProduct/view/20081415091094  
> * 官网定价： 12999 元  

![](http://henjay724.com/image/biweekly/gree_XQG100.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

