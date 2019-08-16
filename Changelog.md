# Soarsea EFI Changelog

English | [中文](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/blob/master/Changelog_CN.md)

- 2019-08-16
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

- 2019-8-7
  - Initial release