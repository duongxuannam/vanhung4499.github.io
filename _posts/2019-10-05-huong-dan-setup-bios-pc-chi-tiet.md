---
title: Hướng dẫn setup bios chi tiết cho một số loại Mainboard PC
tags: bios setup hackintosh
author: Nguyen Van Hung
aside:
  toc: true
---

__Cấu trúc bios utility của mỗi hãng sẽ khác nhau nên mình sẽ chia theo hãng, đối với các main cùng hãng thì đời cũ và đời mới nó cũng không giống nhau hoàn toàn. Trong bài viết này mình chỉ viết hướng dẫn cho các main mới hơn cụ thể là main đi với CPU Intel đầu 6 trở đi.__

## Main Gigabyte
### Setup chung

+ Save & Exit → Load Optimized Defaults
+ M.I.T. → Advanced Memory Settings  Extreme Memory Profile(X.M.P.) : Profile1
+ BIOS → Fast Boot : Disabled
+ BIOS → LAN PXE Boot Option ROM : Disabled
+ BIOS → Storage Boot Option Control : UEFI
+ Peripherals → Trusted Computing → Security Device Support : Disable
+ Peripherals → Network Stack Configuration → Network Stack : Disabled
+ Peripherals → USB Configuration → Legacy USB Support : Auto
+ Peripherals → USB Configuration → XHCI Hand-off : Enabled
+ Chipset → Vt-d : Disabled

### Dành cho card rời
+ Peripherals → Initial Display Output : PCIe 1 Slot
+ Chipset → Integrated Graphics : Disabled

### Dành cho card onboard
+ Peripherals → Initial Display Output : IGFX
+ Chipset → Integrated Graphics : Enabled
+ Chipset → DVMT Pre-Allocated : 128MB

## Main ASRock

### Setup chung
+ OC Tweaker \ DRAM Configuration → Load XMP Setting : XMP 2.0 Profile 1
+ Advanced \ CPU Configuration → Intel Virtualization Technology : Enabled
+ Advanced \ Chipset Configuration → Vt-d : Disabled
+ Advanced \ Storage Configuration → Sata Mode Selection: AHCI
+ Advanced \ Super IO Configuration → Serial Port: Disabled
+ Advanced \ USB Configuration → Legacy USB Support : Enabled
+ Advanced \ USB Configuration → PS/2 Simulator : Disabled
+ Advanced \ USB Configuration → XHCI Hand-off : Enabled
+ Security \ Secure Boot → Secure Boot: Disabled
+ Boot  → Fast Boot: Disabled
+ Boot  → Boot From Onboard LAN: Disabled

### Dành cho card rời
+ Advanced \ Chipset Configuration → Primary Graphics Adapter : PCI Express
+ Advanced \ Chipset Configuration → IGPU Multi-Monitor : Disabled

### Dành cho card onboard
+ Advanced \ Chipset Configuration → Primary Graphics Adapter : Onboard
+ Advanced \ Chipset Configuration → Share Memory : 128MB
+ Advanced \ Chipset Configuration → IGPU Multi-Monitor : Enabled

## Mian ASUS

### Setup Chung
+ Exit → Load Optimized Defaults : Yes
+ Advanced \ CPU Configuration → Intel Virtualizaiton Technology: Enabled
+ Advanced \ System Agent (SA) Configuration → Vt-d: Disabled
+ Advanced \ PCH Configuration → IOAPIC 24-119 Entries: Enabled
+ Advanced \ AMP Configuration → Power On By PCI-E/PCI: Enabled
+ Advanced \ Network Stack Configuration → Network Stack: Disabled
+ Advanced \ USB Configuration -> Legacy USB Support: Auto
+ Boot → Fast Boot : Disabled
+ Boot → Secure Boot → OS Type : Other OS

### Dành cho card rời
+ Advanced \ System Agent (SA) Configuration \ Graphics Configuration → Primary Display: PEG

### Dành cho card onboard
+ Advanced \ System Agent (SA) Configuration \ Graphics Configuration → Primary Display: IGFX
+ Advanced \ System Agent (SA) Configuration \ Graphics Configuration → DVMT Pre-Allocated: 128MB

## Main MSI

### Setup chung
+ Save & Exit → Restore Defaults : Yes
+ Settings \ Advanced \ Integrated Peripherals → Network Stack : [Disabled]
+ Settings \ Advanced \Integrated Peripherals  → Intel Serial IO : [Disabled]
+ Settings \ Advanced \ Integrated Graphics Configuration → DVMT Pre-Allocated : 128MB hoặc 64MB
+ Settings \ Advanced \ USB Configuration → XHCI Hand-off : [Enabled]
+ Settings \ Advanced \ USB Configuration → Legacy USB Support : [Auto]
+ Settings \ Advanced \ Windows OS Configuration → MSI Fast Boot : [Disabled]
+ Settings \ Advanced \ Windows OS Configuration → Fast Boot : [Disabled]
+ Overclocking  → Extreme Memory Profile(X.M.P) : [Enabled]
+ Overclocking \ CPU Features → Intel Virtualization Tech : [Enabled]
+ Overclocking \ CPU Features → Intel VT-D Tech : [Disabled]
+ Settings \ Boot → Boot mode select : [LEGACY+UEFI]

### Dành cho card rời
+ Settings \ Advanced \ Integrated Graphics Configuration → Initiate Graphic Adapter : PEG

### Dành cho card onboard
+ Advanced \ Integrated Graphics Configuration → Initiate Graphic Adapter : IGD

## Boot vào cài đặt
Setup bios xong lưu lại rồi boot usb vào cài đặt thôi.
