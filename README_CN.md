<font color=red>*由于缺少测试的机器，我会逐步停止维护这个项目。如果你对黑苹果有兴趣并希望帮助我维护，请联系我</font>

# S200H-NUC-黑苹果教程

让你的S200H迷你主机吃上黑苹果

[English](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/blob/master/README.md) | 中文

## 配置

| 硬件      | 个人配置                           | 推荐配置 |
| --------- | --------------------------------- | ------- |
| 电脑型号   | S200H NUC mini PC                 | -       |
| 中央处理器 | 英特尔 酷睿 i9-8950HK              | 英特尔 酷睿 i5/i7/i9 (仅支持8-series) |
| 内存      | 镁光 32GB DDR4 2667MHz         | 最低2GB DDR4                         |
| 硬盘      | 三星 970 EVO 1TB               | 最低32GB SATA/NVME SSD               |
| 显卡      | 英特尔 UHD Graphics 630            | 集成显卡或外接AMD独立显卡              |
| 显示器    | LG IPS 全高清 1080p HDMI          | 最低800x600 HDMI/mDP                 |
| 声卡      | 瑞昱 ALC269VC (layout-id:188)     | 内建或USB声卡                        |
| 无线网卡   | 博通 943602CS                    | 博通系列或USB无线网卡                |
| 以太网卡   | 瑞昱 RTL8168H                    | 内建或USB以太网卡                    |

如果需要更多自定义硬件配置，可以向卖家说明购买准系统

## BIOS设置

`Secure Boot` -> `Disabled`  
`VT-d` -> `Enabled`  
`Quiet Boot` -> `Enabled`  
`Fast Boot` -> `Disabled`  
`CSM Support` -> `Disabled`  

## 不正常工作的

- 电源按钮不起作用，强制关机依旧有效
- 显卡问题
  - 睡眠唤醒后部分软件不正常工作（例如 Chrome）
  - 根据[Issues #11](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/11) 和 [Issues #12](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/12)，你可能需要手动添加Fake ID来避免HDMI使用中的黑屏
- 如果发现更多错误，请告诉我

## 支持系统与下载

- macOS High Sierra (仅支持10.13.6)
- macOS Mojave
- macOS Catalina
- Linux
- Windows

[下载最新版](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/releases/download/v1.4/S200H-EFI-v1.4.zip) | [发布](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/releases) | [更新日志](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/blob/master/Changelog_CN.md)

你需要承担尝试预览版后的一切后果，包括任何损害，而不是作者

## 疑难解答

### 进入Clover后无法操作，键盘和鼠标都无响应

如果你遇到这个问题，你可以尝试去BIOS中临时开启`CSM Support`。当你完成macOS的安装后，可以再次尝试关闭此选项

### 部分类似Chrome或Hackintool等软件在电脑从睡眠中唤醒后冻结，并且无法播放视频

目前，这是个普遍和棘手的问题，我尝试和多个黑果专家探讨，暂时还没有得到有效的解决方案

### HEVC编码失效，硬件和BIOS配置都是正常的

根据[Issues #5](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/5)，你可能需要手动下载新版的[Lilu](https://github.com/acidanthera/Lilu/releases) 和 [Whatevergreen](https://github.com/acidanthera/WhateverGreen/releases)，将下载的压缩包解压然后替换`/EFI/CLOVER/Kexts/Other`内原有的kext

### 某些工作负载中出现屏幕花屏或闪屏

幸运的是，大部分用户除了开机时并不会遇到这个问题。这是因为某些显示器通过HDMI连接时可能存在兼容问题，如果你在更换显示器后依旧存在这个问题，请参考[Issues #3](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/3)

### 我可以另加独立显卡吗？英伟达还是AMD？哪个更好？还有我在哪里可以购买扩展坞

英伟达的webdriver并不支持macOS 10.14 Mojave及更高版本，除非你要使用老掉牙的家伙（比如 GT710），否则AMD是更好的选择。如果你不清楚哪个更适合你，请参考[Mojave免驱的A卡](https://github.com/CrazyPegAsus/macOS-Mojave-Compatibility-hardware-list#%E9%A6%96%E9%80%89-%E8%93%9D%E5%AE%9D%E7%9F%B3-%E5%BE%AE%E6%98%9F-%E7%9A%84)。我是在[淘宝官方店](https://item.taobao.com/item.htm?spm=a1z10.5-c-s.w4002-21839614856.41.178472171zqPyZ&id=593258062526)购买的扩展坞，如果感兴趣你也可以自己制作拓展坞。如果需要更多咨询和讨论，请前往[Issues #10](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/10)

### 这个EFI支持macOS的OTA升级吗？ 比如从 10.15.4 到 10.15.5，甚至是以后的 10.16

小版本的OTA更新一般都没问题，但也无法完全避免遇到任何bug甚至是无法开机的情况。你可以尝试在升级前（后）:

1. 暂停macOS的自动更新
2. 确保你已经备份好个人文件
3. 你可以前往各大论坛，或在[Issues](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues)查看有无任何升级成功或失败的报告

由于缺少测试的机器而逐步停更这个项目，对此，我感到十分抱歉！所以对于仅使用这个EFI的用户而言，无痛升级10.16将永不存在（或许会有0.01%）

### 我用这个EFI来跑macOS的时候遇到了问题

你可以去[Issues](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues)查看是否有人遇到了相同的问题，你也可以创建自己发现的问题。欢迎大家给出好的建议和错误反馈

### 有论坛的帖子讨论S200迷你主机的吗

有，我查找了一些论坛，目前找到如下：

- [Tonymacx86](https://www.tonymacx86.com/threads/eglobal-s200-nuc-intel-i7-8750h-mini-pc-compatible.276741)
- [知乎](https://zhuanlan.zhihu.com/p/65263547)
- [远景论坛](http://bbs.pcbeta.com/viewthread-1826798-1-1.html)

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

- 感谢[苹果](https://www.apple.com/) 的 [macOS](https://www.apple.com/macos/)
- 感谢 [RehabMan](https://github.com/RehabMan) 维护的 [EAPD-Codec-Commander](https://github.com/RehabMan/EAPD-Codec-Commander),  [OS-X-Clover-Laptop-Config](https://github.com/RehabMan/OS-X-Clover-Laptop-Config), [OS-X-Null-Ethernet](https://github.com/RehabMan/OS-X-Null-Ethernet), [OS-X-USB-Inject-All](https://github.com/RehabMan/OS-X-USB-Inject-All), 和 [SATA-unsupported](https://github.com/RehabMan/hack-tools/tree/master/kexts/SATA-unsupported.kext)
- 感谢 [Acidanthera](https://github.com/acidanthera) 维护的 [AppleALC](https://github.com/acidanthera/AppleALC), [AppleSupportPkg](https://github.com/acidanthera/AppleSupportPkg), [AptioFixPkg](https://github.com/acidanthera/AptioFixPkg), [HibernationFixup](https://github.com/acidanthera/HibernationFixup), [Lilu](https://github.com/acidanthera/Lilu), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), 和 [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- 感谢 [apianti](https://sourceforge.net/u/apianti), [blackosx](https://sourceforge.net/u/blackosx), [blusseau](https://sourceforge.net/u/blusseau), [dmazar](https://sourceforge.net/u/dmazar), 以及 [slice2009](https://sourceforge.net/u/slice2009) 维护的 [Clover](https://sourceforge.net/projects/cloverefiboot)
- 感谢 [CloverHackyColor](https://github.com/CloverHackyColor) 维护的 [CloverBootloader](https://github.com/CloverHackyColor/CloverBootloader) 和 [CloverThemes](https://github.com/CloverHackyColor/CloverThemes)
- 感谢 [headkaze](https://www.insanelymac.com/forum/profile/1364628-headkaze/) 提供了 [Hackintool](https://github.com/headkaze/Hackintool)
- 感谢 [daliansky](https://github.com/daliansky/Hackintosh) 以及 [stevezhengshiqi](https://github.com/stevezhengshiqi) 提供了大量中文版本的黑苹果资料，和 [GitHub Hackintosh](https://github.com/daliansky/Hackintosh)
- 感谢 [CrazyPegasus](https://github.com/CrazyPegasus) 提供了 [macOS-Mojave-Compatibility-hardware-list](https://github.com/CrazyPegasus/macOS-Mojave-Compatibility-hardware-list)
- 感谢 [kkzzhizhou](https://github.com/kkzzhizhou) 提供了 [USBPorts.kext](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/tree/master/EFI/CLOVER/kexts/Other/USBPorts.kext) 和全部接口的Framebuffer
- 感谢 [Everlasting](https://www.zhihu.com/people/3d7d974acb5eb086a0c378402ae0d100) 提出的无法正常连接4K显示器的问题
- 感谢 [talkmbbs](https://github.com/talkmbbs) 通过 [Issues #2](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/2) 提出的APFS无法引导的问题
- 感谢 [DreamDZhu](https://github.com/DreamDZhu) 通过 [Issues #3](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/3) 提出的屏幕花屏的问题
- 感谢 [MekaYangyi](https://github.com/MekaYangyi) 通过 [Issues #4](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/4) 提出的各个EFI版本的问题
- 感谢 [a22218279](https://github.com/a22218279) 通过 [Issues #5](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/5) 提出的HEVC解码问题
- 感谢 [ciciwind](https://github.com/ciciwind) 通过 [Issues #6](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/6) 提出的OTA升级失败的问题
- 感谢 [imagine243](https://github.com/imagine243) 和 [cdqrain](https://github.com/cdqrain) 通过 [Issues #7](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/7) 和 [Issues #12](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/12) 提出的HDMI连接时屏幕黑屏的问题

## 参考

- [苹果](https://www.apple.com/)
- [谷歌](https://www.google.com/)
- [百度](https://www.baidu.com/)
- [维基百科](https://www.wikipedia.org/)
- [GitHub](https://github.com/)
- [SourceForge](https://sourceforge.net/)
- [InsanelyMac](https://www.insanelymac.com/)
- [TonyMacX86](https://www.tonymacx86.com/)
- [Reddit](https://www.reddit.com/)
- [远景论坛](http://bbs.pcbeta.com/)
- [知乎](https://www.zhihu.com/)
- [淘宝](https://www.taobao.com/)
- [阿里速卖通](https://www.aliexpress.com/)