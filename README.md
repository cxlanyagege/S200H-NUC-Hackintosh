# S200H-NUC-Hackintosh
Installing macOS on your S200H

English | [中文](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/blob/master/README_CN.md)

## Configuration

The following configurations may not be identical. You may ask sellers for a quasi-system if you want more customisations

| Specifications | Details                           |
| -------------- | --------------------------------- |
| PC Model       | S200H NUC mini PC                 |
| Processor      | Intel Core i9/i7/i5               |
| Memory         | 32GB Crucial DDR4 2667MHz         |
| Hard Disk      | Samsung 970 EVO 1TB               |
| Graphics       | Intel UHD Graphics 630            |
| Monitor        | LG IPS Full HD 1080p              |
| Sound Card     | Realtek ALC269VC (layout-id:188)  |
| Wireless Card  | Broadcom 943602CS                 |
| Ethernet       | Realtek RTL8168H                  |

## BIOS Configuration

- Secure Boot -> Disabled
- VT-d -> Enabled
- Quiet Boot -> Enabled
- Fast Boot -> Disabled
- CSM Support -> Disabled

## What is not working

- Power button when host runs macOS
- Some apps may not work after waking up (eg. Chrome etc)
  - I test it out by myself, both HDMI and mDP have this issue
  - According to [Issue #6](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/issues/6), [kkzzhizhou](https://github.com/kkzzhizhou) once experienced randomly apps stucked, just like happened situation after waking up
- Maybe more, you tell me

## Supporting OS & Downloads

- macOS Mojave
- macOS Catalina

[Download latest EFI](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/releases/download/v1.1/S200H-EFI-v1.1.zip) | [Releases](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/releases) | [Changelog](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/blob/master/Changelog.md)

Pre-release should only be tried at your own risk, author would take void on your hardware damages

## Where to buy

- [Taobao](https://item.taobao.com/item.htm?spm=a230r.1.14.20.47f24c1aV8myCD&id=564185703343&ns=1&abbucket=14#detail)
  - If you are not in mainland of China, Taobao may not ship oversea directly. You may need to find agents or someone else takes it from China
- [AliExpress](https://www.aliexpress.com/item/32974757463.html?spm=2114.search0104.3.15.3df35489p80342&ws_ab_test=searchweb0_0,searchweb201602_6_10065_10130_10068_10547_319_317_10548_10696_10192_10190_453_10084_454_10083_10618_10307_10820_10301_10821_10303_537_536_10059_10884_10887_321_322_10103,searchweb201603_52,ppcSwitch_0&algo_expid=7ccf7ab0-f5cf-4f12-95f8-5b616c4e6775-2&algo_pvid=7ccf7ab0-f5cf-4f12-95f8-5b616c4e6775)

## Discussion

- [Tonymacx86](https://www.tonymacx86.com/threads/eglobal-s200-nuc-intel-i7-8750h-mini-pc-compatible.276741)
- [Zhihu](https://zhuanlan.zhihu.com/p/65263547)
  
## Notice

I have decided not to spend too much time on this repo anymore, if someone wants to take it over, please contact me. I may update it once there meets huge updates on macOS, Clover or other kexts

## A reward

The continuous maintenance and updates are all made for free, but you can reward me if you want

| WeChat                                                                                             | Alipay                                                                                             |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| ![Wechat](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/raw/master/Others/Wechat.png) | ![Alipay](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/raw/master/Others/Alipay.jpeg) |


## Credits

- Thanks to [RehabMan](https://github.com/RehabMan) for providing [EAPD-Codec-Commander](https://github.com/RehabMan/EAPD-Codec-Commander),  [OS-X-Clover-Laptop-Config](https://github.com/RehabMan/OS-X-Clover-Laptop-Config), [OS-X-Null-Ethernet](https://github.com/RehabMan/OS-X-Null-Ethernet), [OS-X-USB-Inject-All](https://github.com/RehabMan/OS-X-USB-Inject-All), and [SATA-unsupported](https://github.com/RehabMan/hack-tools/tree/master/kexts/SATA-unsupported.kext)
- Thanks to [Acidanthera](https://github.com/acidanthera) for providing [AppleALC](https://github.com/acidanthera/AppleALC), [AppleSupportPkg](https://github.com/acidanthera/AppleSupportPkg), [AptioFixPkg](https://github.com/acidanthera/AptioFixPkg), [HibernationFixup](https://github.com/acidanthera/HibernationFixup), [Lilu](https://github.com/acidanthera/Lilu), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), and [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
- Thanks to [apianti](https://sourceforge.net/u/apianti), [blackosx](https://sourceforge.net/u/blackosx), [blusseau](https://sourceforge.net/u/blusseau), [dmazar](https://sourceforge.net/u/dmazar), and [slice2009](https://sourceforge.net/u/slice2009) for providing [Clover](https://sourceforge.net/projects/cloverefiboot)
- Thanks to [kkzzhizhou](https://github.com/kkzzhizhou) for providing [USBPorts.kext](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/tree/master/EFI/CLOVER/kexts/Other/USBPorts.kext) and Framebuffer for both HDMI and DP port
- Thanks to [daliansky](https://github.com/daliansky/Hackintosh) and [stevezhengshiqi](https://github.com/stevezhengshiqi) for providing basic Chinese Hackintosh stencil and [Hackintool](https://github.com/daliansky/Hackintosh)
- Thanks to [Everlasting](https://www.zhihu.com/people/3d7d974acb5eb086a0c378402ae0d100) for indicating the failure when connecting to a 4K monitor
