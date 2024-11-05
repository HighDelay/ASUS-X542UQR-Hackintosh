# ASUS-X542UQR-Hackintosh

```
Specs
CPU: i5 8250U Kabylake-R 
GPU: Intel UHD 620
GPU2: Nvidia Geforce 940MX
```

**Hackintosh Ventura, Sonoma, and Sequoia / Opencore 1.0.2 / Asus Vivobook 15 X542UQ"R"**

This EFI works best with Ventura, Sonoma, and Sequoia, so I will only be updating OC but not 
the OS. **Perhaps**

config.plist was configured based on [this guide](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html)

**SMBIOS:** MacBookPro15,2 /w working CPU PM + CPUFriend & USB mapping using 
[USBMap](https://github.com/corpnewt/USBMap)

Sleep only works with the power adapter unplugged.

Replace the wifi card with "Intel Dual Band Wireless-AC 3165"

Turn `CFG Lock` and `VT-d` off via modGRUBShell

Voltageshift (CPU Undervolting): `./voltageshift buildlaunchd -99.6 0 -99.6 0 0 0 1 15 15 0 120`

# Screenshots
![1](/SC/1.png)
![2](/SC/2.png)
![3](/SC/3.png)
