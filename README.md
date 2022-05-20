# Clevo-N960SC-N960SDS-N960SF1-Hackintosh

## 简介

Clevo-N960SC-N960SDS-N960SF1-Hackintosh UEFI通过OC启动，支持任意版本系统OTA升级到最新系统

## 硬件支持情况

1. 内置键盘和数字键盘
2. 原生USB3.0/USB2.0 
3. AppleHDA原生音频（包括耳机）
4. 内置摄像头
5. 原生电源管理电池状态
6. 核显驱动
7. 有线以太网卡
8. Mac App Store正常运行
9. CPU变频
10. 睡眠唤醒
11. 无线网络触控板（全系支持全手势）
12. 随航（有线/无线）支持休眠唤醒

## Bios修改项（可能需要解锁bios隐藏有风险）



### bios禁用

**CFG Lock**（bios直接关闭或者使用OpenCore 选单中的GRUB Shell，回车进入命令行，输入，回车，然后退出setup_var 0x3E 0x0exit关闭CFG Lock后需要将配置文件中和两项Quirks 禁用config.plistAppleCpuPmCfgLockAppleXcpmCfgLock）

**SGX**

**Fastboot**

**VT-d**

**Platform Trust**

## 开启HIDPI（Big Sur及以上）

**启动终端输入：**

```shell
bash -c "$(curl -fsSL https://raw.githubusercontent.com/xzhih/one-key-hidpi/master/hidpi.sh)"
```
