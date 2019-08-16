# Soarsea-i9-8950HK-Hackintosh
Installing macOS on your Soarsea mini PC (S200H)

English | [中文](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/blob/master/README_CN.md)

## Configuration

The following configurations may not be identical. You may ask sellers for a quasi-system if you want more customization

| Specifications | Details                           |
| -------------- | --------------------------------- |
| PC Model       | Soarsea mini PC                   |
| Processor      | Intel Core i9-8950HK              |
| Memory         | 32GB Crucial DDR4 2667MHz         |
| Hard Disk      | Samsung 970 EVO 1TB               |
| Graphics       | Intel UHD Graphics 630            |
| Monitor        | LG IPS Full HD 1080p              |
| Sound Card     | Realtek ALC 269VC (layout-id:188) |
| Wireless Card  | Broadcom 943602CS                 |
| Ethernet       | Realtek RTL8168H                  |

## Supported macOS Versions

- macOS Mojave
- macOS Catalina Beta

## What is not working

- Power button when host runs macOS
- Some apps may not work after waking up from sleeping (Chrome etc.)
  - According to [tonymacx86.com](https://www.tonymacx86.com/threads/eglobal-s200-nuc-intel-i7-8750h-mini-pc-compatible.276741/page-4), this situation only appears when connecting display by HDMI. I would confirm this later once I get a adapter for mDP to VGA and move it to "Notice", since there had been already such a lot of people concentrating on it without any solution so far yet
- Maybe more, you tell me

## Where to buy

- [Taobao](https://item.taobao.com/item.htm?spm=a230r.1.14.20.47f24c1aV8myCD&id=564185703343&ns=1&abbucket=14#detail)
  - If you are not in mainland of China, Taobao does not ship oversea directly. You may need to find agents or someone else takes it from China

## Changelog

You can view [Changelog](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/blob/master/Changelog.md) for more detailed release information
  
## Notice

- Generally, i5 and i7 models will work fine by using this EFI file directly, but I have not tested them yet, please trying themselves at your own risk
- I use BCM943602CS in M.2 Key M slot instead of native card slot, the USB bus should work according to [kkzzhizhou](https://github.com/kkzzhizhou)'s report, if it does not work, please go to "Issues"

## Credits

- Thanks to [kkzzhizhou](https://github.com/kkzzhizhou) for providing [USBPorts.kext](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/tree/master/EFI/CLOVER/kexts/Other/USBPorts.kext) and Framebuffer for both HDMI and DP port
