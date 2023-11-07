# ASUS-X542UQR-Hackintosh

```
Specs
CPU: i5 8250U Kabylake-R 
GPU: Intel UHD 620
GPU2: Nvidia Geforce 940MX
```

**Hackintosh Ventura & Sonoma / Opencore 0.9.6 / Asus Vivobook 15 X542UQ"R"**

This EFI works best with Ventura & Sonoma, and mainly Sonoma, so I will only be updating OC but not 
the OS. **Perhaps**

**Note for Sonoma (11/7/2023):** Turned out spoofing iGPU wasn't necessary

config.plist was configured based on [this guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html)

**SMBIOS:** MacBookPro15,2 /w working CPU PM + CPUFriend & USB mapping using 
[USBMap](https://github.com/corpnewt/USBMap)

Sleep only works with the power adapter unplugged.

Replaced the wifi card with "Intel Dual Band Wireless-AC 3165" For Sonoma, use [Bluetooth](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/issues/437#issuecomment-1579931908)

Voltageshift (CPU Undervolting): `./voltageshift buildlaunchd -99.6 0 -99.6 0 0 0 1 15 15 0 120`

# Screenshots
![1](/SC/1.png)
![2](/SC/2.png)
![3](/SC/3.png)
