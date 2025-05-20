# TridentOS

This is a silly little project. Do not expect it to work.

## Prerequisites

The project requires a Unix-like environment. If you are using Windows, there are various ways of setting one up (WSL, a Linux virtual machine, Cygwin, MSYS2). I recommend using WSL, which is the [easiest to setup](https://learn.microsoft.com/en-us/windows/wsl/install).

You need the following tools:

* `make`
* `nasm`
* Open Watcom
* `qemu-system-x86` for testing
* `bochs-x bochsbios vgabios` for debugging
* your preferred text editor

### Installing Open Watcom

1. Download [the latest build for Linux](https://github.com/open-watcom/open-watcom-v2/releases)
1. Run the installer with sudo (the downloaded file is executable)
1. When prompted for what components to install, select "Selective installation" and enable "Include 16-bit compilers"
1. If you installed the 64-bit version, in `Makefile` and `src/bootloader/stage2/Makefile` modify the `CC16` and `LD16` variables to point to `/usr/bin/watcom/binl64/wcc` and `/usr/bin/watcom/binl64/wlink`. If you modified the installation path, set the correct paths.

## Build instructions

* run `make`

## Running with qemu

* run `./run.sh`

## Debugging with bochs

* run `./debug.sh`

**Troubleshooting**: Bochs has proven to be pretty unreliable. Check [this article](https://github.com/nanobyte-dev/nanobyte_os/wiki/Frequent-issues#bochs-doesnt-work) for some troubleshooting tips.
