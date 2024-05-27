## ROG STRIX B760-A GAMING WiFi Hackintosh OpenCore EFI

![image](ScreenShot/ROGB760A.jpg)

### [简体中文](README.zh_CN.md)

### OpenCore

[OpenCore 1.0.0](https://github.com/acidanthera/OpenCorePkg)

### OS Version Tested

- macOS Monterey 12.x
- macOS Ventura    13.x
- macOS Sonoma   14.x 

### Hardware

- Motherboard: Asus ROG Strix B760-A Gaming WiFi
- Bios Version:1641（2024/02/20）
- CPU: Intel i7-13700KF
- RAM: G.SKILL 32GB*2 DDR5 6400MHz
- SSD: 1.ZHITAI Ti600 1TB MacOS
- SSD: 2.KINGSTON SKC3000D 2048G Windows
- GPU: ASUS AMD Radeon RX6600XT 8GB
- Ethernet Card: Intel L226-V
- WiFi Card: Intel Wi-Fi 6E AX211 160MHz

### Notes

 - Use [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools) build your SMBIOS
 - If you want to use a CPU without  Efficient-Core, you must uncheck the option in the config.plist file Kernel--ProvideCurrentCpuinfo
 - Intel WiFi driver [AirportItlwm.kext](https://github.com/OpenIntelWireless/itlwm/releases) in this EFI is only applicable to MacOS 14.4 - 14.5 Sonoma. Please download and replace this driver yourself when installing other MacOS versions

### Bios Setup

```
Advanced

  |-- UEFI Variables Protection
     |-- password protection of Runtime Variables ：Disabled
     
  |-- System Agent(SA)Configuration
     |-- VT-D ：Enabled
     |-- Control Iommu Pre-boot Behavior ：Disable IOMMU
	   
  |--PCI Subsystem Settings
     |-- Above 4G Decoding ：Enabled
     |-- Resize BAR Support ：Disabled
     |-- SR-IOV Support ：Disabled
   
Boot

  |-- Secure Boot
    |-- OS Type ：Other OS
    |-- Secure Boot Mode ：Custom
      
  |-- Boot Configuration
    |-- Fast Boot ：Disabled
      
  |-- CSM (Compatibility Support Module)
    |-- Launch CSM  ：Disabled
	
```


### Contact Us

 - QQ Group: 23304408

![image](ScreenShot/QRCode.png)