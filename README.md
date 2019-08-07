# Soarsea-i9-8950HK-Hackintosh
Pathway for tasting macOS on your Soarsea mini PC

## Configuration

The following configurations may not be identical. You may ask sellers for a quasi-system if you want more customization

| Specifications | Details                           |
| -------------- | --------------------------------- |
| PC Model       | Soarsea mini PC                   |
| Processor      | Intel Core i9-8950HK / i7 / i5    |
| Memory         | 32GB Crucial DDR4 2667MHz         |
| Hard Disk      | Samsung 970 EVO 1TB               |
| Graphics       | Intel UHD Graphics 630            |
| Monitor        | LG IPS FullHD 1080p               |
| Sound Card     | Realtek ALC 269VC (layout-id:188) |
| Wireless Card  | Broadcom 943602CS                 |

## Supported macOS Versions

- macOS High Sierra 10.13.6 (DID NOT TEST)
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

- i5 and i7 models mat not work
  - I did not test other CPU models, trying these at your own risk
- Power button when host runs macOS
- Slightly artifacts when booting into the second stage
- Some USB ports may not work
  - I use BCM943602CS in M.2 Key M slot instead of native card slot, the USB bus should work according to [kkzzhizhou](https://github.com/kkzzhizhou)'s report
- Display Port is not working
  - I use HDMI, you can modify "Framebuffer" to enable DP port
- HDMI Audio may not work
  - Did not test it yet
- USB Keyboard does not work well
  - As for me, it happens, still pending
- Maybe more, you tell me

## Credits

- Thanks to [kkzzhizhou](https://github.com/kkzzhizhou) for providing [USBPorts.kext](https://github.com/kkzzhizhou/S200H_I7-8750H_Hackintosh/tree/master/EFI/CLOVER/kexts/Other/USBPorts.kext)
