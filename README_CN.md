# Soarsea-i9-8950HK-黑苹果教程
让你的深水宝迷你主机吃上黑苹果

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

## 正常工作

- Clover正常引导与启动
- 原生CPU电源管理
- 原生显卡驱动，QE/CI水波纹
- 原生睡眠与电能小熹
- 原生内建声卡通道
- 原生NVME SSD支持
- 原生无线网络，蓝牙与以太网网络
- USB正常工作，已使用USBPorts.kext禁用多余通道

## 不正常工作

- 电源按钮不起作用
- 启动到第二阶段一瞬间会有花屏
- 睡眠唤醒后部分软件不正常工作（Chrome等）
- 若有未发现的错误，请报告给我

## 购买途径

- [Taobao](https://item.taobao.com/item.htm?spm=a230r.1.14.20.47f24c1aV8myCD&id=564185703343&ns=1&abbucket=14#detail)
  
## 注意事项

- 通常情况下，i5或i7的型号可以直接使用这份EFI文件，但我并没有专门测试它，你需要承担一切责任来测试是否在你的机器上工作
- 我的BCM943602CS目前使用转接板插在M2 SSD插槽上（Key M通道不带USB通道，目前我用的外接蓝牙），所以我无法测试默认网卡槽的蓝牙通道是否正确开启，根据[kkzzhizhou](https://github.com/kkzzhizhou)的测试结果应该没有问题，如果蓝牙意外不工作，请前往“Issues”报告问题
- 由于使用和测试环境的限制，我只使用了HDMI，如果你需要DP，你可以自行修改Framebuffer
- 不久前刚刚开启了国外留学之旅，适应期间，更新速度与部分基础测试准备可能不尽人意，希望理解，圣诞节过后应该会更好些，我太难了

## 感谢

- 感谢 [kkzzhizhou](https://github.com/kkzzhizhou) 提供了 [USBPorts.kext](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/tree/master/EFI/CLOVER/kexts/Other/USBPorts.kext)
