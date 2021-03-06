# Thinkpad T450s Catalina
## 简介
- 这是一个完整的Thinkpad T450s macOS Catalina配置 （基于 @jsassu20 的T450配置）
- 由于T450s只有一条内存插槽（使用8GB以上内存时板载内存识别不正常）您需要注入内存信息
- 使用DW1820A时只需将驱动复制到kext 安装系统时无需在BIOS中禁用WIFI
- 音频问题请执行alc_fix脚本 或者把CodecCommander.kext复制到 L / E 目录重建缓存修复权限
## 硬件信息

```  
- CPU：Intel Core i7-5600U 2.6GHz (Boots 3.2GHz)

- 核心显卡：Intel HD 5500 Graphics 

- 声卡：ALC292

- 无线网卡：DW1820A CN-08PKF4 CN-0VW3T3 CN-00JT494（感谢 @Axelpop ）
```

## BIOS
- `Security -> Security Chip`: **Disabled**;
- `Memory Protection -> Execution Prevention`: **Enabled**;
- `Virtualization -> Intel Virtualization Technology`: **Enabled**;
- `Internal Device Access -> Bottom Cover Tamper Detection`: must be **Disabled**;
- `Anti-Theft -> Current Setting`: **Disabled**;
- `Anti-Theft -> Computrace -> Current Setting`: **Disabled**;
- `Secure Boot -> Secure Boot`: **Disabled**;
- `UEFI/Legacy Boot`: **UEFI Only**;
- `CSM Support`: **Yes**.

## 有效

- 睡眠/唤醒
- Wifi
- 蓝牙 
- Handoff, Continuity, AirDrop
- iMessage, FaceTime, App Store, iTunes Store
- 以太网卡
- 板载音频 (使用alc_fix或CodecCommander.kext修复音频问题)
- USB
- 电池
- 触摸屏 (10.14)
- 触摸板
- 小红点
- miniDP
- SD卡读卡器

## 无效

- VGA
- 触摸屏 (10.15)
