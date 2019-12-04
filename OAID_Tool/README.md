# Get_Oaid_CNAdid

[TOC]



## 背景

随 Android Q 的到来，IMEI 无法获取，获取稳定的 ID 成为越来越多的开发者迫切需求。

本项目，将行业中两个替代 ID —— OAID 和 CNAdid 的获取方法提供给大家。

其中 OAID 是由手机厂联盟提供的广告跟踪标示，CNAdid 是数字联盟“可信 ID ”的免费版。  



## 声明

OAID 移动安全联盟（该联盟为**中国信息通信研究院**下属**电信终端产业协会**的下属联盟组织）联合终端厂商推出的团体标准，该标准目前正在申报中，尚未申请成功。

 OAID：**Open Anonymous** Device Identifier **开放**匿名设备标识符

根据该联盟公布在网上的《移动智能终端补充设备标识规范》文本“本规范旨在规范移动智能终端补充设备标识体系的体系架构、功能要求、接口要求以及安全要求。 **规范设备生产企业遵循标准要求开发统一接口调用方式，方便移动应用接入、减小维护成本”**。因此该联盟及者联盟单位必须将统一的 OAID 调用方式公布出来，这也是“中华人民共和国标准化法”的法律要求。事实上，除非是**企业内部标准**，其他标准都**必须**公开。

**根据标准法的第二十二条：**

制定标准应当有利于科学合理利用资源，推广科学技术成果，增强产品的安全性、通用性、可替换性，提高经济效益、社会效益、生态效益，做到技术上先进、经济上合理。 **禁止利用标准实施妨碍商品、服务自由流通等排除、限制市场竞争的行为。**

作为商用 ID 服务商，良性竞争能够让我们的产品变得更好，考虑到不是所有企业都有能力购买数字联盟的可信 ID 系统，但对于设备标示又有需求，因此数字联盟将在本项目中，将各类设备的 OAID 调用方式，发布出来以方便开发者使用同时也提供可信 ID 的免费版本 CNAdid 的调用方式。详细介绍见（[www.cnadid.cn）](http://www.cnadid.cn)




## 支持功能

OAID 目前提供一下设备的获取方式:
小米、vivo、华为、OPPO、Lenovo、华硕、三星、魅族、努比亚

CNAdid目前提供安卓全平台获取方式。  



## 支持范围（具体支持时间看厂商的正式公告）

| 厂商   | 版本                                  |
| ------ | ------------------------------------- |
| 小米   | MIUI10.2 及以上                       |
| vivo   | FuntouchOS 9 及以上                   |
| 华为   | 全版本                                |
| OPPO   | Color OS 7.0 及以上（10月份正式支持） |
| Lenovo | ZUI 11.4 及以上（10月中旬正式支持）   |
| 华硕   | Android Q（10月份会正式支持）         |
| 魅族   | 10月份将支持                          |
| 三星   | 10月份将支持                          |
| 努比亚 | 10月份将支持                          |



## 标识特性

**OAID（匿名设备标识符）重置特性**

发生下述事件时，OAID（匿名设备标识符）重置:

(1) 用户在系统设置中手动重置，匿名设备标识符将重置;
(2) 移动智能终端恢复出厂设置时，匿名设备标识符将重置;
(3) 匿名设备标识符自身可定期重置。 重置后生成新的匿名设备标识符，且应用只能获取新的匿名设备标识符。

**匿名设备标识符的开启\关闭受控机制**
移动智能终端应提供匿名设备标识符的开启\关闭受控机制，用户可以选择在系统设置中关闭匿名 设备标识符；关闭后，应用获取到的匿名设备标识符的返回值为 NO。

**请注意：**OAID 与IMEI 不同，IMEI 为设备标示，对于相同设备在不被篡改时，不发生变化，可以作为画像索引 key。
OAID 为广告标识，同一台设备在不同时间内，可以拥有不同的的 OAID，因此无法作为稳定的索引key 使用。详细信息参考（[www.msa-alliance.cn）](http://16054554.s21d-16.faiusrd.com/0/ABUIABA9GAAgpKaN6QUoq7em2QI?f=%E5%9B%A2%E4%BD%93%E6%A0%87%E5%87%86-%E7%A7%BB%E5%8A%A8%E6%99%BA%E8%83%BD%E7%BB%88%E7%AB%AF%E8%A1%A5%E5%85%85%E8%AE%BE%E5%A4%87%E6%A0%87%E8%AF%86%E8%A7%84%E8%8C%83-v20190516.pdf&amp;v=1562596132)

CNAdid 为稳定设备标示，有良好的反作弊对抗特征，详细信息参考（[www.cnadid.cn)](http://www.cnadid.cn%29/)  



## 截图展示

![1](D:\GitLabProjects\open-source\OAID_Tool\images\1.png)    ![2](D:\GitLabProjects\open-source\OAID_Tool\images\2.png)
