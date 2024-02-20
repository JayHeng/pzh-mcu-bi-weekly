# 痞子衡嵌入式半月刊： 第 92 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 91 期》](https://www.cnblogs.com/henjay724/p/18013504)

## 唠两句

历史上的今天：1986年2月20日，被命名为“蜜蜂六号”的我国第一艘热飞艇在北京试飞成功，填补了我国飞行器在这一项目的空白。

本期共收录 1 条资讯、5 个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、瑞萨电子宣布收购PCB设计软件Altium</font>

日本瑞萨电子近日宣布，将以59亿美元现金收购电子设计公司 Altium，致力于为客户提供数字设备设计。Altium 成立于1985年，是全球第一家PCB设计工具供货商。

 * 资讯来源：https://www.renesas.cn/cn/zh/about/press-room/renesas-acquire-pcb-design-software-leader-altium-make-electronics-design-accessible-broader-market

瑞萨电子一直与 Altium 合作，Altium 的 PCB 设计软件添加了世界上第一个用于设计和实现电子硬件的数字平台 Altium 365，在整个 PCB 设计过程中实现了无缝协作。2023 年 6 月，瑞萨电子宣布在 Altium 365 云平台上实现了所有 PCB 设计的标准化开发，将其所有产品的 ECAD 库发布到 Altium Public Vault。借助 Altium365 上的制造商零件搜索等功能，客户可以直接从 Altium 库中选择瑞萨电子零件，以加快上市速度。

## 项目类

### <font color="red">1、probe-rs - 嵌入式调试和目标交互的工具包</font>

probe-rs 是一个嵌入式调试和目标交互的工具包，它使用户可以对微控制器进行编程和调试。

 * 项目地址：https://github.com/probe-rs/probe-rs

probe-rs 用于实现来自不同制造商和不同芯片架构的硬件调试器的协议。它的目标是提供一个工具集来与各种嵌入式MCU和调试探针进行交互。类似的项目如 OpenOCD、PyOCD、Segger Toolset、ST Tooling等也存在。它们都实现了GDB协议和它们自己的协议，以使GDB能够与调试探针通信。probe-rs 项目去掉了GDB层，并提供了一个到调试探针的直接接口，从而使其他软件能够使用其调试功能。

### <font color="red">2、uthash - 一个为C语言提供哈希表的库</font>

uthash 是为 C 语言提供哈希表功能的库。由于标准 C 语言中没有类似字典的数据结构，该库提供了哈希表常见的查询、插入、删除、排序等函数。uthash 使用方法非常简单，仅需引入一个头文件即可。

 * 项目地址：https://github.com/troydhanson/uthash

```C
#include "uthash.h"

struct my_struct {
    int id;            /* we'll use this field as the key */
    char name[10];
    UT_hash_handle hh; /* makes this structure hashable */
};

struct my_struct *users = NULL;

void add_user(struct my_struct *s) {
    HASH_ADD_INT( users, id, s );
}
```

### <font color="red">3、chibicc - 一个实现了大多数C11特性的小型C编译器</font>

chibicc 是一个实现了大多数 C11 特性的小型 C 编译器。尽管它可能仍然像其他小型编译器一样被归为“玩具编译器”类别，但 chibicc 可以编译几个真实的程序，包括 Git、SQLite、libpng 和 chibicc 本身，而无需对编译的程序进行修改。这些程序生成的可执行文件通过相应的测试套件。因此，chibicc 实际上支持各种各样的 C11 特性，并且能够正确编译数十万行真实的C代码。

 * 项目地址：https://github.com/rui314/chibicc

这个项目的每次提交都与作者编写的书里章节有关。为此，不仅项目的最终状态，而且每次提交都是仔细编写的，并考虑到可读性。读者能够通过阅读这个项目的一个或几个提交来了解如何实现C语言特性。例如，这就是while、[]、?:和线程局部变量的实现方式。

### <font color="red">4、TinySSH - 一个极简的SSH服务器实现</font>

tinysshd 是一个简约的 SSH 服务器，它只实现了SSHv2功能的一个子集。它支持安全加密(最低128位安全性，防止缓存定时攻击)，不实现旧的加密(如RSA, DSA, HMAC-MD5, HMAC-SHA1, 3DES, RC4，…)，不实现不安全的特性(如密码或基于主机的身份验证)，也没有SSH1协议、压缩、端口转发、代理转发、X11转发等功能，未使用动态内存分配(没有分配失败等)。

 * 项目地址：https://github.com/janmojzis/tinyssh

 ### <font color="red">5、Quadsort - 一种比快速排序快且稳定的归并排序算法</font>

Quadsort 是一种比快速排序快，稳定的归并排序算法。项目包含原理讲解、C 语言实现、性能对比和排序过程。

 * 项目地址：https://github.com/scandum/quadsort

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-092/Quadsort.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

