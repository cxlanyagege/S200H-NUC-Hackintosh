# Soarsea-i9-8950HK-Hackintosh
Installing macOS on your Soarsea mini PC (S200H)

English | [中文](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/blob/master/README_CN.md)

## Configuration

The following configurations may not be identical. You may ask sellers for a quasi-system if you want more customisations

| Specifications | Details                           |
| -------------- | --------------------------------- |
| PC Model       | Soarsea mini PC                   |
| Processor      | Intel Core i9-8950HK              |
| Memory         | 32GB Crucial DDR4 2667MHz         |
| Hard Disk      | Samsung 970 EVO 1TB               |
| Graphics       | Intel UHD Graphics 630            |
| Monitor        | LG IPS Full HD 1080p              |
| Sound Card     | Realtek ALC269VC (layout-id:188) |
| Wireless Card  | Broadcom 943602CS                 |
| Ethernet       | Realtek RTL8168H                  |

## What is not working

- Power button when host runs macOS
- Some apps may not work after waking up from sleeping (Chrome etc.)
  - According to [tonymacx86.com](https://www.tonymacx86.com/threads/eglobal-s200-nuc-intel-i7-8750h-mini-pc-compatible.276741/page-4), this situation only appears when connecting display by HDMI. I would confirm this later once I get a adapter for mDP to VGA and move it to "Notice", since there had been already such a lot of people concentrating on it without any solution so far yet
  - According to [Issue #6](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/issues/6), [kkzzhizhou](https://github.com/kkzzhizhou) once experienced randomly apps stucked, just like happened situation after waking up
- Maybe more, you tell me

## Where to buy

- [Taobao](https://item.taobao.com/item.htm?spm=a230r.1.14.20.47f24c1aV8myCD&id=564185703343&ns=1&abbucket=14#detail)
  - If you are not in mainland of China, Taobao may not ship oversea directly. You may need to find agents or someone else takes it from China

## Supports & Downloads

- macOS Mojave
- macOS Catalina

[Download latest](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/releases/download/v1.1/Soarsea-EFI-v1.1.zip) | [Releases](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/releases) | [Changelog](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/blob/master/Changelog.md)
  
## Notice

- Generally, i5 and i7 models will work fine by using this EFI file directly, but I have not tested them yet, please trying themselves at your own risk
- I use BCM943602CS in M.2 Key M slot instead of native card slot, the USB bus should work according to [kkzzhizhou](https://github.com/kkzzhizhou)'s report, if it does not work, please go to "Issues"

## A reward

The continues maintenance and release are all made for free, but you can reward me if you want

| WeChat                                                                                             | Alipay                                                                                             |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| ![Wechat](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/raw/master/Others/Wechat.png) | ![Alipay](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/raw/master/Others/Alipay.jpeg) |


## Credits

- Thanks to [RehabMan](https://github.com/RehabMan) for providing [EAPD-Codec-Commander](https://github.com/RehabMan/EAPD-Codec-Commander),  [OS-X-Clover-Laptop-Config](https://github.com/RehabMan/OS-X-Clover-Laptop-Config), [OS-X-Null-Ethernet](https://github.com/RehabMan/OS-X-Null-Ethernet), [OS-X-USB-Inject-All](https://github.com/RehabMan/OS-X-USB-Inject-All), and [SATA-unsupported](https://github.com/RehabMan/hack-tools/tree/master/kexts/SATA-unsupported.kext)
- Thanks to [Acidanthera](https://github.com/acidanthera) for providing [AppleALC](https://github.com/acidanthera/AppleALC), [AppleSupportPkg](https://github.com/acidanthera/AppleSupportPkg), [AptioFixPkg](https://github.com/acidanthera/AptioFixPkg), [HibernationFixup](https://github.com/acidanthera/HibernationFixup), [Lilu](https://github.com/acidanthera/Lilu), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), and [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- Thanks to [apianti](https://sourceforge.net/u/apianti), [blackosx](https://sourceforge.net/u/blackosx), [blusseau](https://sourceforge.net/u/blusseau), [dmazar](https://sourceforge.net/u/dmazar), and [slice2009](https://sourceforge.net/u/slice2009) for providing [Clover](https://sourceforge.net/projects/cloverefiboot)
- Thanks to [kkzzhizhou](https://github.com/kkzzhizhou) for providing [USBPorts.kext](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/tree/master/EFI/CLOVER/kexts/Other/USBPorts.kext) and Framebuffer for both HDMI and DP port
- Thanks to [daliansky](https://github.com/daliansky/Hackintosh) and [stevezhengshiqi](https://github.com/stevezhengshiqi) for providing basic Chinese Hackintosh stencil and [Hackintool](https://github.com/daliansky/Hackintosh)
