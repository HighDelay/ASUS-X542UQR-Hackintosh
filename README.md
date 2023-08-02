# X542UQR-Hackintosh

```
Specs
CPU: i5 8250U Kabylake-R
GPU: Intel UHD 620
GPU2: Nvidia Geforce 940MX
```

Opencore 0.9.3

config.plist was configured based on [this guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html)

SMBIOS: MacBookPro15,2 /w working CPU PM + CPUFriend & USB mapping using 
[USBMap](https://github.com/corpnewt/USBMap)


This EFI works best with Ventura & Sonoma so I will only be updating OC but not 
the OS. **Perhaps**

**Note for Sonoma (8/2/2023):** MacOS Sonoma no longer supports any 2017 Macbook models that have Intel Kabylake CPUs in them, which means drivers for Kabylake iGPU will be removed. However, at the moment I'm writing this, MacOS Sonoma is still in the beta stage, and drivers and kexts for Kabylake iGPU are still there and work fine, but there is a high chance that they will be removed when the beta is over. So you should keep yourself posted on the repo, I'm going to update it (spoof the iGPU to Coffelake equivalent) when an official release of MacOS Sonoma comes out. If the drivers are still available, I'll leave it as is.

Sleep only works with the power adapter unplugged.

Replaced the wifi card with "Intel Dual Band Wireless-AC 3165"

Voltageshift (CPU Undervolting): `./voltageshift buildlaunchd -99.6 0 -99.6 0 0 0 1 15 15 0 120`
