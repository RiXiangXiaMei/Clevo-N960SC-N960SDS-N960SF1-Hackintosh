# Clevo-N960SC-N960SDS-N960SF1-Hackintosh
Clevo-N960SC / N960SDS / N960SF1-Hackintosh
UEFI通过OC 启动
支持任意版本系统OTA升级到最新系统
内置键盘以及数字键盘
原生USB3.0/USB2.0
AppleHDA原生音频，包括耳机
内置摄像头
原生电源管理
电池状态
核显驱动
有线以太网卡
Mac App Store 正常运行
CPU变频
睡眠唤醒
无线网络
触控板（全系支持全手势）
随航（有线/无线）
支持休眠唤醒


关闭 CFG Lock：使用 OpenCore 选单中的 GRUB Shell，回车进入命令行，输入，回车，然后退出setup_var 0x3E 0x0exit
关闭 CFG Lock之后需要将配置文件中和两项 Quirks 禁用config.plistAppleCpuPmCfgLockAppleXcpmCfgLock

可选项目（需要在 BIOS 中通过文件启动 GRUB Shell 来调出完整选项，输入）：禁用 SGX、Fastboot、VT-d、Platform Trust（下面是 BIOS 中的位置）setup_var 0x133 0x1
SGX、快速启动、VT-d：高级->高级芯片组控制
平台信任：高级 -> 芯片组配置
开启 HIDPI（Big Sur及以上）：bash -c "$(curl -fsSL https://raw.githubusercontent.com/xzhih/one-key-hidpi/dev/hidpi.sh)"
支持 macOS Monterey Developer Beta（OTA）
