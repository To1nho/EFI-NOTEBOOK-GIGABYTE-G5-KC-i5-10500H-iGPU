# Gigabyte G5-KC Hackintosh

![seggs](https://github.com/To1nho/EFI-NOTEBOOK-GIGABYTE-G5-KC-i5-10500H-iGPU/blob/main/System%20Information/sysinfow.png)![seggs](https://github.com/To1nho/EFI-NOTEBOOK-GIGABYTE-G5-KC-i5-10500H-iGPU/blob/main/System%20Information/sysinfob.png)

# Basic Information

**Latest working macOS**: macOS Ventura (13.5.2)
<br>
**Current OpenCore**: 0.9.5
<br>
**Release date**: 18/09/2023

## Specification of this machine:
| Hardware  | Name of this | Note |
| ------------- | ------------- | ------------- |
| CPU | [Intel Core i5-10500H](https://www.intel.com/content/www/us/en/products/sku/201905/intel-core-i510500h-processor-12m-cache-up-to-4-50-ghz/specifications.html)  |
| Memory | 16GB Dual-Channel |
| GPU 1 | Integrated Intel UHD Graphics |
| GPU 2 | NVIDIA RTX 3060 6GB | Unsupported in macOS |
| Ethernet (LAN) | Realtek RTL8111 |
| Wireless (WLAN) | Intel Wi-Fi 6 AX200 | You should replace this part if you want to use AirDrop Function |
| Audio | Realtek ALC293 |
| Storage 1 | NVME SX8200PNP-512GT-S 512GB|
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
| Screen output (HDMI, DP) | ⭕ ... | Only MiniDP works because it's connected to the iGPU |
| Sleep | ✔️ Working | Disable hibernate. |

## Something you must read before using this EFI Template:
1. Please do research your computer (Hardware, Software, PC Model...)

3. If you want to use AirDrop/Hand-off/Continuity function, please replace your wireless card inside your laptop. [Wireless Buyer Guide](https://dortania.github.io/Wireless-Buyers-Guide/)
- ***I haven't included wireless kext in this EFI, so you need to do it manually.***

4. Change BIOS Setting as Dortania's Guide: [BIOS Setting](https://github.com/dortania/oc-laptop-guide-legacy/blob/master/before-you-start/bios-configuration.md)
