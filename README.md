# ASUS-X542UQR-Hackintosh

```
Specs
CPU: i5 8250U Kabylake-R 
GPU: Intel UHD 620 (Spoofed as Coffeelake's Intel UHD 630 for Sonoma)
GPU2: Nvidia Geforce 940MX
```

**Hackintosh Ventura & Sonoma / Opencore 0.9.3 / Asus Vivobook 15 X542UQ"R"**

This EFI works best with Ventura & Sonoma so I will only be updating OC but not 
the OS. **Perhaps**

~~**Note for Sonoma (8/2/2023):** MacOS Sonoma no longer supports any 2017 Macbook models that have Intel Kabylake CPUs in them, which means drivers for Kabylake iGPU will be removed. However, at the moment I'm writing this, MacOS Sonoma is still in the beta stage, and drivers and kexts for Kabylake iGPU are still there and work fine, but there is a high chance that they will be removed when the beta is over. So you should keep yourself posted on the repo, I'm going to update it (spoof the iGPU to Coffelake equivalent) when an official release of MacOS Sonoma comes out. If the drivers are still available, I'll leave it as is.~~

**Note for Sonoma (8/3/2023):** Spoofed the iGPU as Coffeelake's Intel UHD 630. However, this causes changing the laptop screen's brightness to not work (Max brightness on default).

**To fix black screen no backlight add this to `boot-args`**
```
-igfxblt for Sonoma (Default)
-igfxblr for Ventura 
```
config.plist was configured based on [this guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html)

**SMBIOS:** MacBookPro15,2 /w working CPU PM + CPUFriend & USB mapping using 
[USBMap](https://github.com/corpnewt/USBMap)

Sleep only works with the power adapter unplugged.

Replaced the wifi card with "Intel Dual Band Wireless-AC 3165" For Sonoma, use [This version of Itlwm](https://github.com/OpenIntelWireless/itlwm/issues/883#issuecomment-1639920021) + [Bluetooth](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/issues/437#issuecomment-1579931908)

Voltageshift (CPU Undervolting): `./voltageshift buildlaunchd -99.6 0 -99.6 0 0 0 1 15 15 0 120`

# Screenshots
![1](/SC/1.png)
![2](/SC/2.png)
![3](/SC/3.png)
