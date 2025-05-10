# Trident
## About
Trident is a lightweight operating system for (currently) legacy BIOS systems with the goal of future support for UEFI and basic networking capabilities. It will be entirely free-standing, with it's own graphics library, kernel, bootloader, everything. It will also be entirely modular, making it easy to customise whilst not being bloated.

---
## Development
You can help develop Trident using the [Trident Cross Compiler](https://github.com/gingrspacecadet/TCC).

---
## Features 
* [x] Bootable BIOS system using GRUB (Eventually will use custom)
* [x] Basic kernel
* [x] VGA text printing
* [ ] Paging
* [ ] Multithreading
* [ ] Interupts
* [ ] Timers
* [ ] Keyboard Input
* [ ] Mouse Input
* [ ] Physical Memory Management
* [ ] Virtual Memory Management
* [ ] Heap Allocation

---
## License
MIT license

---
## Prerequisites
* UNIX-like operating system (To build it)
* QEMU or another hypervisor (If virtualising)
* Bourne-Again Shell (BASH)

---
## Disclaimer
Trident is a passion project, and is unlikely to be stable. Installing it on real hardware is a bad idea. Also, it isn't finished, so if there is something missing either make it yourself and pull request or suck it up.