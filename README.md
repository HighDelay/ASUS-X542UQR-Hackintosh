# X542UQR-Hackintosh

```
Specs
CPU: i5 8250U
GPU: Intel UHD 620
GPU2: Nvidia Geforce 940MX
```

Opencore 0.8.9

config.plist were configured based on [this guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html)

SMBIOS: MacBookPro14,1 /w working CPU PM + CPUFriend & USB mapping using 
[USBMap](https://github.com/corpnewt/USBMap)


This EFI works best with Ventura, so I will only be updating OC but not 
the OS. **Perhaps**

Sleep only works with the power adapter unplugged.

Replaced the wifi card with "Intel Dual Band Wireless-AC 3165"

Voltageshift: `./voltageshift buildlaunchd -99.6 0 -99.6 0 0 0 1 15 15 0 120`
