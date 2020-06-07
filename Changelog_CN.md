# S200H EFI 更新日志

[English](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/blob/master/Changelog.md) | 中文

- 2020-06-07 v1.4
  - 支持 macOS Catalina 10.15.5 (感谢 [chenyucheng0503](https://github.com/chenyucheng0503) 与 [xanadu314](https://github.com/xanadu314) 反馈 [Issues #11](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/11))
  - 更新 `Clover` 5119
  - 更新 `Lilu` 1.4.5
  - 更新 `AppleALC` 1.5.0
  - 更新 `Whatevergreen` 1.4.0
  - 更新 `VirtualSMC` 1.1.4, including `SMCProcessor` and `SMCSuperIO`
  - 更新 `ApfsDriverLoader.efi` `AudioDxe.efi` `DataHubDxe.efi` `FSInject.efi`
  - 更新内建的 `UEFI Shell`
  - 移除部分在tool文件夹内无用的二进制包

- 2020-03-28 v1.3
  - 支持 macOS Catalina 10.15.4 （感谢 [ciciwind](https://github.com/ciciwind) 反馈 [Issues #6](https://github.com/EngLearnsh/S200H-NUC-Hackintosh/issues/6)）
  - 更新 `Clover` 5107
  - 更新 `Lilu` 1.4.2
  - 更新 `AppleALC` 1.4.7
  - 更新 `Whatevergreen` 1.3.7
  - 更新 `VirtualSMC` 1.1.1, 包括 `SMCProcessor` and `SMCSuperIO`
  - 更新 `ApfsDriverLoader.efi` `AudioDxe.efi` `DataHubDxe.efi` `FSInject.efi`
  - 更新内建的 `UEFI Shell`

- 2019-12-22 v1.2
  - 更新 `Clover` 5101
  - 更新 `Lilu` 1.4.0
  - 更新 `AppleALC` 1.4.4
  - 更新 `Whatevergreen` 1.3.5
  - 更新 `VirtualSMC` 1.0.9，包括两个传感器驱动
  - 更新 `ApfsDriverLoader.efi`，解决部分分区引导问题
  - 支持4K分辨率输出
  - 移除 `framebuffer-fbmem` 和 `framebuffer-stolenmem` 以改善显卡的稳定性
  - 移除无用的主题

- 2019-11-19 v1.2 Beta 2
  - 更新 `Clover` 5098
  - 更新 `Lilu` 1.3.9
  - 更新 `AppleALC` 1.4.3
  - 更新 `Whatevergreen` 1.3.4
  - 更新 `VirtualSMC` 1.0.9，包括两个传感器驱动
  - 更新 `ApfsDriverLoader.efi`，解决部分分区引导问题
  - 移除无用的主题

- 2019-09-04 v1.2 Beta 1
  - 支持4K分辨率
  - 移除 `framebuffer-fbmem`, `framebuffer-stolenmem` 和 `framebuffer-unifiedmem` 以测试显卡的稳定性

- 2019-08-16
  - 更新 `Clover` 5045
  - 更新 `Lilu` 1.3.8
  - 更新 `AppleALC` 1.4.0
  - 更新 `Whatevergreen` 1.3.1
  - 更新 `VirtualSMC` 1.0.7, 包括两个传感器驱动
  - 修复系统启动到第二阶段时的花屏
  - 修复 Display port, 现在HDMI和DP都可以使用了 (感谢 kkzzhizhou)
  - 改善高分辨率屏幕的显示效果
  - 移除 `SSDT-DEHCI`, `SSDT-DEH01`, `SSDT-DEH02`, `SSDT-IMEI` 因为它们会引发ACPI错误
  - 移除 DSDT 重命名项目 `Change HECI to IMEI` 因为它并无实质性作用
  - 增加 `AddDTGP` 和 `AddIMEI` 的修复, 现在启动速度会比之前快一半
  - 增加 PCI 设备属性, 从而让macOS可以更好地识别它们
  - 减少Clover启动等待时间到2秒

- 2019-08-07
  - 初版发布