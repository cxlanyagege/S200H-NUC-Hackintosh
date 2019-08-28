# Soarsea-i9-8950HK-黑苹果教程
让你的深水宝迷你主机吃上黑苹果 (S200H)

[English](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/blob/master/README.md) | 中文

## 配置

以下配置并非与卖家预配描述完全一致，如果需要更多自定义硬件配置，可以向卖家说明购买准系统

| 硬件      | 规格                               |
| --------- | --------------------------------- |
| 电脑型号   | Soarsea mini PC                   |
| 中央处理器 | Intel Core i9-8950HK              |
| 内存      | 32GB Crucial DDR4 2667MHz         |
| 硬盘      | Samsung 970 EVO 1TB               |
| 显卡      | Intel UHD Graphics 630            |
| 显示器    | LG IPS Full HD 1080p              |
| 声卡      | Realtek ALC269VC (layout-id:188)  |
| 无线网卡   | Broadcom 943602CS                 |
| 以太网卡   | Realtek RTL8168H                  |

## 不正常工作

- 电源按钮不起作用
- 睡眠唤醒后部分软件不正常工作（Chrome等）
  - 根据[tonymacx86.com](https://www.tonymacx86.com/threads/eglobal-s200-nuc-intel-i7-8750h-mini-pc-compatible.276741/page-4)上的汇报，该问题只出现在HDMI连接上，一旦我有mDP转VGA转换线并测试证实后，我会把这个问题放到“注意事项”中，因为它已经足够被其他购买者重视，但至今仍未有解决方案
  - 根据[Issue #6](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/issues/6), [kkzzhizhou](https://github.com/kkzzhizhou)在正常使用情况下遇到过与睡眠唤醒后一样的现象
- 若发现更多错误，请报告给我

## 购买途径

- [淘宝](https://item.taobao.com/item.htm?spm=a230r.1.14.20.47f24c1aV8myCD&id=564185703343&ns=1&abbucket=14#detail)

## 支持与下载

- macOS Mojave
- macOS Catalina

[下载最新版](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/releases/download/v1.1/Soarsea-EFI-v1.1.zip) | [发布](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/releases) | [更新日志](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/blob/master/Changelog.md)
  
## 注意事项

- 通常情况下，i5或i7的型号可以直接使用这份EFI文件，但我并没有专门测试它，你需要承担一切责任来测试是否在你的机器上工作
- 我的BCM943602CS目前使用转接板插在M2 SSD插槽上（Key M通道不带USB通道，目前我用的外接蓝牙），所以我无法测试默认网卡槽的蓝牙通道是否正确开启，根据[kkzzhizhou](https://github.com/kkzzhizhou)的测试结果应该没有问题，如果蓝牙意外不工作，请前往“Issues”报告问题

## 捐赠

所有持续更新与正式版发布均免费，如果你认可我的工作，欢迎给我买瓶冰红茶

| 微信                                                                                             | 支付宝                                                                                             |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| ![Wechat](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/raw/master/Others/Wechat.png) | ![Alipay](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/raw/master/Others/Alipay.jpeg) |

## 鸣谢

- 感谢 [RehabMan](https://github.com/RehabMan) 提供了 [EAPD-Codec-Commander](https://github.com/RehabMan/EAPD-Codec-Commander),  [OS-X-Clover-Laptop-Config](https://github.com/RehabMan/OS-X-Clover-Laptop-Config), [OS-X-Null-Ethernet](https://github.com/RehabMan/OS-X-Null-Ethernet), [OS-X-USB-Inject-All](https://github.com/RehabMan/OS-X-USB-Inject-All), 和 [SATA-unsupported](https://github.com/RehabMan/hack-tools/tree/master/kexts/SATA-unsupported.kext)
- 感谢 [Acidanthera](https://github.com/acidanthera) 提供了 [AppleALC](https://github.com/acidanthera/AppleALC), [AppleSupportPkg](https://github.com/acidanthera/AppleSupportPkg), [AptioFixPkg](https://github.com/acidanthera/AptioFixPkg), [HibernationFixup](https://github.com/acidanthera/HibernationFixup), [Lilu](https://github.com/acidanthera/Lilu), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), 和 [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- 感谢 [apianti](https://sourceforge.net/u/apianti), [blackosx](https://sourceforge.net/u/blackosx), [blusseau](https://sourceforge.net/u/blusseau), [dmazar](https://sourceforge.net/u/dmazar), 以及 [slice2009](https://sourceforge.net/u/slice2009) 提供了 [Clover](https://sourceforge.net/projects/cloverefiboot)
- 感谢 [kkzzhizhou](https://github.com/kkzzhizhou) 提供了 [USBPorts.kext](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/tree/master/EFI/CLOVER/kexts/Other/USBPorts.kext) 和全部接口的Framebuffer
- 感谢 [daliansky](https://github.com/daliansky/Hackintosh) 以及 [stevezhengshiqi](https://github.com/stevezhengshiqi) 提供了大量中文版本的黑苹果资料，和 [Hackintool](https://github.com/daliansky/Hackintosh)
