# 痞子衡嵌入式半月刊： 第 102 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 101 期》](https://www.cnblogs.com/henjay724/p/18214344)

## 唠两句

历史上的今天：

本期共 2 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、eepromfs - 基于EEPROM的简易类文件数据读写库</font>

eepromfs 是一个基于 EEPROM 的简易类文件的数据读写库，方便做动态功能增减时参数管理，增减参数块类似增减文件，不会对已有数据存储带来影响，适合在 EEPROM 硬件资源充裕的情况下使用。

该库设计的核心思想是 EPPROM 存储区开头存储 eepromfs 管理相关信息，采用链表方式串联每一个文件，每个文件建立的时候指定名称和大小，新增加的文件自动追加在链表末尾。该科可以在大部分嵌入式 arm 下使用，硬件需要带 eeprom，建议采用 24C256、24c512 之类的大容量芯片。

 * 项目地址：https://gitee.com/wtau_zaozao/eepromfs

### <font color="red">2、PDHV - 可调高压USB PD电源</font>

PDHV 是一个可调 300V 高压 USB PD 电源，所有 USB 端口都彼此隔离并与高压隔离。

 * 项目地址：https://github.com/Aylo6061/PDHV

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-102/PHDV.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

