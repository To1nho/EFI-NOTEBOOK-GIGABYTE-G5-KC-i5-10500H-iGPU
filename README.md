# Gigabyte G5-KC Hackintosh

![seggs](https://github.com/quynkk1/G5KC-Hackintosh/blob/main/giga.jpg)

## Specification of this machine:
| Hardware  | Name of this | Note |
| ------------- | ------------- | ------------- |
| CPU | [Intel Core i5-10500H 6-Core](https://www.intel.com/content/www/us/en/products/sku/201905/intel-core-i510500h-processor-12m-cache-up-to-4-50-ghz/specifications.html)  |
| Memory | 16GB A-DATA Memory  |
| GPU 1 | Integrated Intel UHD Graphics  |
| GPU 2 | NVIDIA RTX 3060 6GB | Unsupported in macOS |
| Ethernet (LAN) | Realtek RTL8168/8111 |
| Wireless (WLAN) | Intel Wi-Fi 6 AX200 | You should replace this part if you want to use AirDrop Function |
| Audio | Realtek ALC293 |
| Storage 1 | NVMe ESR512GTLCG-EAC-4  |
| Storage 2 | TOSHIBA MK3265GSX HDD  |
| Keyboard | Standard PS/2 Keyboard |
| Touchpad | Intel I2C HID |

## What's working ? 
| Peripherals | Status | Note |
| ------------- | ------------- | ------------- |
| Power Management | ✔️ Working |  |
| Graphics Accelerator (Intel UHD) | ✔️ Working |  |
| Graphics Accelerator (NVIDIA RTX) | ❌ ... | RTX is not supported by Apple. |
| Internet | ✔️ Working | Both Wi-Fi and LAN working well |
| Audio output | ✔️ Working | Both Internal speaker, headphones and micro |
| Keyboard and mouse | ✔️ Working | Either volume and function key or trackpad |
| Camera | ✔️ Working |  |
| Battery and AC | ⭕ ... | Read below |
| USB Ports | ✔️ Working | Both Type-A and Type-C |
| Screen output (HDMI, DP) | ⭕ ... | Just MiniDP works because it's conectet on iGPU |
| Sleep | ✔️ Working | Disable hibernate. |

## Something you must read before using this EFI Template:
1. Please do research your computer (Hardware, Software, PC Model...)
2. Battery status is a BIG ISSUE and I have no idea to fix this. Conclusion below:

| Battery status 🔋 | Things happened | 
| ------------- | ------------- |
| Only run with battery | Battery reported correct percentage |
| Low battery (Under 10%) | Battery reported correct percentage and show low battery notification  |
| Battery in charge mode (AC Adapter plugged) | Battery icon reported **"Power Source: Battery"** |
| Battery in charge mode (AC Adapter plugged) and restarted PC | Battery icon still reported **"Power Source: Battery"** |

Note: Battery light lighted up when I plugged AC Adapter

3. If you want to use AirDrop/Hand-off/Continuity function, please replace your wireless card inside your laptop. [Wireless Buyer Guide](https://dortania.github.io/Wireless-Buyers-Guide/)
- ***I haven't included wireless kext in this EFI, so you need to do it manually.***

4. Change BIOS Setting as Dortania's Guide: [BIOS Setting](https://github.com/dortania/oc-laptop-guide-legacy/blob/master/before-you-start/bios-configuration.md)
## Thanks to:
[Apple](apple.com) for [macOS](https://en.wikipedia.org/wiki/MacOS)

[Acidanthera](https://github.com/acidanthera) for [OpenCore](https://github.com/acidanthera/OpenCorePkg) and relevant kernel extension

... and other developer :3

