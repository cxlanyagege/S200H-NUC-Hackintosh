# Soarsea-i9-8950HK-Hackintosh
Pathway for tasting macOS on your Soarsea mini PC

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

## What is working

- Regular boot by Clover
- Native CPU power management
- Native GPU, full QE/CI
- Native Sleep / PowerNap
- Native built-in sould
- Native NVMe SSD Support
- Native WIFI / Bluetooth / Ethernet
- USB3.0 / 2.0 / Type-C works fine, limited useless ports by USBPorts.kext

## What is not working

- Power button when host runs macOS
- Slightly artifacts when booting into the second stage
- Display Port is not working
  - I use HDMI, you can modify "Framebuffer" to enable DP port
- HDMI Audio may not work
  - Have not test it yet
- Maybe more, you tell me

## Where to buy

- [Taobao](https://item.taobao.com/item.htm?spm=a230r.1.14.20.47f24c1aV8myCD&id=564185703343&ns=1&abbucket=14#detail)
  - If you are not in mainland of China, Taobao does not ship oversea directly. You may need to find agents or someone else takes it from China
  
## Notice

- Generally, i5 and i7 models will work fine by using this EFI file directly, but I have not tested them yet, please trying themselves at your own risk
- I use BCM943602CS in M.2 Key M slot instead of native card slot, the USB bus should work according to [kkzzhizhou](https://github.com/kkzzhizhou)'s report, if it does not work, please go to "Issues"

## Credits

- Thanks to [kkzzhizhou](https://github.com/kkzzhizhou) for providing [USBPorts.kext](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/tree/master/EFI/CLOVER/kexts/Other/USBPorts.kext)
