# Hackintosh-Dell-Precision-m4600

CLOVER folder for to install MacOS for Dell Precision m4600

Tested on: macOS Sierra

### My Specs:

CPU: i7-2620M, 3200 MHz

RAM: 8GB DDR3

Motherboard Chipset: Intel Cougar Point QM67, Intel Sandy Bridge

GPU: NVIDIA Quadro 2000M

Sound: IDT 92HD90BXX

Monitor: Samsung 156AT (Dell C54GW) 15,6" HD

LAN: Intel(R) 82579LM Gigabit Network Connection

WIFI: Intel(R) Centrino(R) Ultimate-N 6300 AGN

### What's working

- Full SpeedStep CPU (without patching ssdt)

- GPU fully supported

- Sound: AppleHDA working using [this patch](https://github.com/insanelydeepak/Patched-AppleHDA-for-Mac-OS-Sierra-10.12)

- Shutdown

- Ethernet

- USB2.0, USB3.0

### Not yet working:

- SD Card slot

- Stock Wi-fi card

- Sleep

- Bluetooth

- Touchpad

- VGA/HDMI

### Prerequisites

- USB MacOS Sierra installer

- BIOS: AHCI mode -> SATA

- BIOS: Secure boot -> disabled

- Your disk should be converted from LEGACY to UEFI (if not) using Minitool Partition

### Install

- Clone/Download this repo and rename the repo's folder to **CLOVER**, and put in boot partition -> *EFI* folder

- Add Clover boot loader file **\EFI\CLOVER\CLOVERX64.efi** to UEFI boot list

- Boot into Clover, select your USB, create a Mac partition and install MacOS ( If you get stuck while booting to installer, try to boot with flag: nv_disable=1 )

### Post-install

- Download your favorite kext installer app like [this](http://www.insanelymac.com/forum/files/file/397-easykext-pro-a-minimal-and-super-fast-kext-installer/)

- Download and install newest [VoodooPS2Controller](https://github.com/RehabMan/OS-X-Voodoo-PS2-Controller)

- Download and install [Patched AppleHDA](https://github.com/insanelydeepak/Patched-AppleHDA-for-Mac-OS-Sierra-10.12)

- If USB3.0/Battery/Ethernet not working, install ACPIBatteryManager, GenericUSBXHCI, IntelMausiEthernet and restart


_Any pull request would be appreciated_
