# Soarsea-i9-8950HK-黑苹果教程
让你的深水宝迷你主机吃上黑苹果 (S200H)

[English](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/blob/master/README.md) | [中文](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/blob/master/README_CN.md)

## 配置

以下配置并非与卖家预配描述完全一致，如果需要更多自定义硬件配置，可以向卖家说明购买准系统

| 规格      | 细节                               |
| --------- | --------------------------------- |
| 电脑型号   | Soarsea mini PC                   |
| 中央处理器 | Intel Core i9-8950HK              |
| 内存      | 32GB Crucial DDR4 2667MHz         |
| 硬盘      | Samsung 970 EVO 1TB               |
| 显卡      | Intel UHD Graphics 630            |
| 显示器    | LG IPS Full HD 1080p              |
| 声卡      | Realtek ALC 269VC (layout-id:188) |
| 无线网卡   | Broadcom 943602CS                 |
| 以太网卡   | Realtek RTL8168H                  |

## 支持的macOS版本

- macOS Mojave
- macOS Catalina Beta

## 不正常工作

- 电源按钮不起作用
- 睡眠唤醒后部分软件不正常工作（Chrome等）
- 若发现更多错误，请报告给我

## 购买途径

- [淘宝](https://item.taobao.com/item.htm?spm=a230r.1.14.20.47f24c1aV8myCD&id=564185703343&ns=1&abbucket=14#detail)
  
## 注意事项

- 通常情况下，i5或i7的型号可以直接使用这份EFI文件，但我并没有专门测试它，你需要承担一切责任来测试是否在你的机器上工作
- 我的BCM943602CS目前使用转接板插在M2 SSD插槽上（Key M通道不带USB通道，目前我用的外接蓝牙），所以我无法测试默认网卡槽的蓝牙通道是否正确开启，根据[kkzzhizhou](https://github.com/kkzzhizhou)的测试结果应该没有问题，如果蓝牙意外不工作，请前往“Issues”报告问题

## 感谢

- 感谢 [kkzzhizhou](https://github.com/kkzzhizhou) 提供了 [USBPorts.kext](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/tree/master/EFI/CLOVER/kexts/Other/USBPorts.kext) 和全部接口的Framebuffer
