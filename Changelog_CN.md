# Soarsea EFI 更新日志

[English](https://github.com/EngLearnsh/Soarsea-i9-8950HK-Hackintosh/blob/master/Changelog.md) | 中文

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

- 2019-8-7
  - 初版发布