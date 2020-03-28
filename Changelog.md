# S200H EFI Changelog

English | [中文](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/blob/master/Changelog_CN.md)

- 2020-03-28 v1.3
  - Support macOS Catalina 10.15.4 (Thanks to [ciciwind](https://github.com/ciciwind) via [Issues #6](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/6))
  - Update `Clover` 5107
  - Update `Lilu` 1.4.2
  - Update `AppleALC` 1.4.7
  - Update `Whatevergreen` 1.3.7
  - Update `VirtualSMC` 1.1.1, including `SMCProcessor` and `SMCSuperIO`
  - Update `ApfsDriverLoader.efi` `AudioDxe.efi` `DataHubDxe.efi` `FSInject.efi`
  - Update built-in `UEFI Shell`


- 2019-12-22 v1.2
  - Update `Clover` 5101
  - Update `Lilu` 1.4.0
  - Update `AppleALC` 1.4.4
  - Update `Whatevergreen` 1.3.5
  - Update `VirtualSMC` 1.0.9, including two sensor kexts
  - Update `ApfsDriverLoader.efi`, solving some volume guiding problems
  - Support 4K resolution output
  - Remove `framebuffer-fbmem` and `framebuffer-stolenmem`to improve stability on graphics
  - Remove useless themes

- 2019-11-19 v1.2 Beta 2
  - Update `Clover` 5098
  - Update `Lilu` 1.3.9
  - Update `AppleALC` 1.4.3
  - Update `Whatevergreen` 1.3.4
  - Update `VirtualSMC` 1.0.9, including two sensor kexts
  - Update `ApfsDriverLoader.efi`, solving some volume guiding problems
  - Remove useless themes

- 2019-09-04 v1.2 Beta 1
  - Support 4K resolution
  - Remove `framebuffer-fbmem`, `framebuffer-stolenmem` and `framebuffer-unifiedmem` to test stability on graphics

- 2019-08-16 v1.1
  - Update `Clover` 5045
  - Update `Lilu` 1.3.8
  - Update `AppleALC` 1.4.0
  - Update `Whatevergreen` 1.3.1
  - Update `VirtualSMC` 1.0.7, including two sensor kexts
  - Fix artifacts when boot into 2nd stage
  - Fix Display port, now both HDMI and DP will work (credit to kkzzhizhou)
  - Improve graphics effect for high resolution displays
  - Remove `SSDT-DEHCI`, `SSDT-DEH01`, `SSDT-DEH02`, `SSDT-IMEI` since they will cause ACPI errors
  - Remove DSDT rename of `Change HECI to IMEI` since it has no impacts
  - Add `AddDTGP` and `AddIMEI` fixes, boot up speed is now 50% faster
  - Add PCI devices properties, which will have a better indication in macOS for these devices
  - Decrease boot volume selection timeout to 2 seconds

- 2019-08-07 v1.0
  - Initial release