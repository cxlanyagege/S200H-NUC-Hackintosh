# S200H-NUC-黑苹果教程
让你的S200H迷你主机吃上黑苹果

[English](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/blob/master/README.md) | 中文

## 配置

以下是我的个人运行良好的配置。如果需要更多自定义硬件配置，可以向卖家说明购买准系统

| 硬件      | 个人配置                           | 推荐配置 |
| --------- | --------------------------------- | ------- |
| 电脑型号   | S200H NUC mini PC                 | -       |
| 中央处理器 | 英特尔 酷睿 i9-8950HK              | Intel Core i5/i7/i9 (8-series only) |
| 内存      | 镁光 32GB DDR4 2667MHz         | 最低2GB DDR4                         |
| 硬盘      | 三星 970 EVO 1TB               | 最低32GB SATA/NVME SSD               |
| 显卡      | 英特尔 UHD Graphics 630            | 集成显卡或外接AMD独立显卡              |
| 显示器    | LG IPS 全高清 1080p HDMI          | 最低800x600 HDMI/mDP                 |
| 声卡      | 瑞昱 ALC269VC (layout-id:188)     | 内建或USB声卡                        |
| 无线网卡   | 博通 943602CS                    | 博通系列或USB无线网卡                |
| 以太网卡   | 瑞昱 RTL8168H                    | 内建或USB以太网卡                    |

## BIOS设置

`Secure Boot` -> `Disabled`  
`VT-d` -> `Enabled`  
`Quiet Boot` -> `Enabled`  
`Fast Boot` -> `Disabled`  
`CSM Support` -> `Disabled`  

## 不正常工作的

- 电源按钮不起作用
- 睡眠唤醒后部分软件不正常工作（Chrome等）
  - 经过我的测试，HDMI和mDP都有此问题
  - 根据[Issue #6](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/issues/6), [kkzzhizhou](https://github.com/kkzzhizhou)在正常使用情况下遇到过与睡眠唤醒后一样的现象
- 若发现更多错误，请告诉我

## 支持系统与下载

- macOS High Sierra (只支持10.13.6)
- macOS Mojave
- macOS Catalina

[下载最新版](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/releases/download/v1.4/S200H-EFI-v1.4.zip) | [发布](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/releases) | [更新日志](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/blob/master/Changelog_CN.md)

你需要承担尝试预览版后的一切后果，包括任何损害，而不是作者

## 疑难解答

### 进入Clover后无法操作，键盘和鼠标都无响应

如果你遇到这个问题，你可以尝试去BIOS中临时开启`CSM Support`。当你完成macOS的安装后，可以再次尝试关闭此选项

### 部分类似Chrome或Hackintool等软件在电脑从睡眠中唤醒后冻结，并且无法播放视频

目前，这是个普遍和棘手的问题，我尝试和多个黑果专家探讨，暂时还没有得到有效的解决方案

### 我用这个EFI来跑macOS的时候遇到了问题

你可以去[Issues](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues)查看是否有人遇到了相同的问题，你也可以创建自己发现的问题。欢迎大家给出好的建议和错误反馈

### 有论坛的帖子讨论S200迷你主机的吗

有，我查找了一些论坛，目前找到如下：

- [Tonymacx86](https://www.tonymacx86.com/threads/eglobal-s200-nuc-intel-i7-8750h-mini-pc-compatible.276741)
- [知乎](https://zhuanlan.zhihu.com/p/65263547)

### 我在哪儿可以买S200迷你主机

卖家和本人没有任何关系，我的工作是为S200迷你主机创造一个良好的黑果环境

- [淘宝](https://item.taobao.com/item.htm?spm=a230r.1.14.20.47f24c1aV8myCD&id=564185703343&ns=1&abbucket=14#detail)
- [阿里速卖通](https://www.aliexpress.com/item/32974757463.html?spm=2114.search0104.3.15.3df35489p80342&ws_ab_test=searchweb0_0,searchweb201602_6_10065_10130_10068_10547_319_317_10548_10696_10192_10190_453_10084_454_10083_10618_10307_10820_10301_10821_10303_537_536_10059_10884_10887_321_322_10103,searchweb201603_52,ppcSwitch_0&algo_expid=7ccf7ab0-f5cf-4f12-95f8-5b616c4e6775-2&algo_pvid=7ccf7ab0-f5cf-4f12-95f8-5b616c4e6775)

## 捐赠

所有持续更新与正式版发布均免费，如果你认可我的工作，欢迎给我买瓶冰红茶

| 微信                                                                                             | 支付宝                                                                                             |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| ![Wechat](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/raw/master/Others/Wechat.png) | ![Alipay](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/raw/master/Others/Alipay.jpeg) |

## 鸣谢

- 感谢 [RehabMan](https://github.com/RehabMan) 提供了 [EAPD-Codec-Commander](https://github.com/RehabMan/EAPD-Codec-Commander),  [OS-X-Clover-Laptop-Config](https://github.com/RehabMan/OS-X-Clover-Laptop-Config), [OS-X-Null-Ethernet](https://github.com/RehabMan/OS-X-Null-Ethernet), [OS-X-USB-Inject-All](https://github.com/RehabMan/OS-X-USB-Inject-All), 和 [SATA-unsupported](https://github.com/RehabMan/hack-tools/tree/master/kexts/SATA-unsupported.kext)
- 感谢 [Acidanthera](https://github.com/acidanthera) 提供了 [AppleALC](https://github.com/acidanthera/AppleALC), [AppleSupportPkg](https://github.com/acidanthera/AppleSupportPkg), [AptioFixPkg](https://github.com/acidanthera/AptioFixPkg), [HibernationFixup](https://github.com/acidanthera/HibernationFixup), [Lilu](https://github.com/acidanthera/Lilu), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), 和 [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- 感谢 [apianti](https://sourceforge.net/u/apianti), [blackosx](https://sourceforge.net/u/blackosx), [blusseau](https://sourceforge.net/u/blusseau), [dmazar](https://sourceforge.net/u/dmazar), 以及 [slice2009](https://sourceforge.net/u/slice2009) 提供了 [Clover](https://sourceforge.net/projects/cloverefiboot)
- 感谢 [kkzzhizhou](https://github.com/kkzzhizhou) 提供了 [USBPorts.kext](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/tree/master/EFI/CLOVER/kexts/Other/USBPorts.kext) 和全部接口的Framebuffer
- 感谢 [daliansky](https://github.com/daliansky/Hackintosh) 以及 [stevezhengshiqi](https://github.com/stevezhengshiqi) 提供了大量中文版本的黑苹果资料，和 [Hackintool](https://github.com/daliansky/Hackintosh)
- 感谢 [Everlasting](https://www.zhihu.com/people/3d7d974acb5eb086a0c378402ae0d100) 提出的无法正常连接4K显示器的问题
