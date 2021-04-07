# Deskmini H310 黑苹果 启动EFI OC 版

OpenCore 版本: `0.6.8`
驱动基本完美, 无不良情况出现。
<br>

## Mac OS

MacOS Big Sur: `11.2.3`
<br>


## Hardwares

- CPU: I9-9900T QS 版本
- 内存：16Gx2 32G
- 网卡：白果卡 BCM943602CS + 转接卡
- 硬盘：东芝 KIOXIA RC10 500G
<br>


## BIOS Settings

  - CPU Configuration, CPU C states Support, Enabled,
  - CPU Configuration, CPU C states Support, CFG Lock Disabled (必须）
  - Chipset Configuration, Vt-d, Disabled,
  - Chipset Configuration, Onboard HD Audio: Enabled,
  - USB Configuration, XHCI Hand-off, Enabled  （关键）
  - Super IO Configuration, Serial Port, Disabled（必须）
  - Security Secure Boot, Disabled(by default)
  - Boot, CSM, disabled
  - BIOS版本必须在4.0及以上！
<br>


# Misc

- 系统完成后睡眠修复, 打开终端执行:

  ```bash
  sudo pmset standby 0
  sudo pmset autopoweroff 0
  sudo pmset hibernatemode 0
  sudo pmset proximitywake 0
  ```
> 或者使用 Hackintool 电源部分修复.

<br>


- 系统偏好设置: 节能

   - 取消勾选: 唤醒以供以太网络访问
