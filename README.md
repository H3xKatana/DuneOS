

# Dune OS

Dune OS is a Debian-based Linux distribution optimized for educational purposes, featuring KDE Plasma with custom configurations and branding.

## System Requirements

- **Processor**: 64-bit architecture (x86_64)
- **RAM**: Minimum 2 GB (4 GB recommended)
- **Disk Space**: 20 GB minimum
- **Graphics**: GPU with OpenGL 2.0+ support

## Features

- **Base**: Debian (Stable) forked from mint os
- **Desktop Environment**: KDE Plasma, pre-configured with performance and usability tweaks
- **Package Manager**: `APT` with additional custom repositories
- **Kernel**: Linux 6.15
- **File System**: ext4 by default, supports btrfs, xfs, etc.
- **Display Manager**: SDDM
- **Boot Loader**: GRUB2

## Installation Instructions

1. **Download ISO**:
**Currently, only the OEM entry in the boot menu is functional. The remaining entries will be implemented and corrected in future updates**
   - Obtain the latest ISO from (here)[https://drive.google.com/drive/folders/1_zsP1eXjTQZbHpIxg45RFBib5f6w9OcG]
2. **Create Bootable USB**:
   
   - Or use tools like Rufus, Etcher, etc.

3. **Boot from USB**:
   - Restart your system and select the boot device (USB) from the BIOS/UEFI menu.

4. **Install Dune OS**:
   - Follow the on-screen instructions in the Ubiquity installer:
   - install the gpu drivers
     - Select partitioning scheme (manual or guided).
     - Configure user, time zone, and keyboard layout.
     - Begin installation.

6. **Post-Installation**:
   - After installation, the system will reboot. Log in using your created credentials. ( dune : dune )
  

## System Customizations

- **KDE Plasma**:
  - Pre-configured with a custom theme, layout, and Dune OS-specific tweaks for optimized performance on low-resource systems.
  - Custom wallpapers and branding.
- ** LIST of Software **
  - IDE/code editors :VS code , code blocks , eclipse 
  - Networking : wireshark , cisco packettracer
  - office : libreoffice
  - others : GDB , cutter , github desktop , gitq , qemu virtual manger , virtualbox 


## Package Management

- **Updating the System**:
  ```bash
  sudo apt update && sudo apt full-upgrade
  ```

- **Adding Software**:
  ```bash
  sudo apt install <package-name>
  ```

- **Removing Software**:
  ```bash
  sudo apt remove <package-name>
  ```

## Services and Optimization

- **Disabled Unnecessary Services**:
  - Optimized system services to reduce resource usage on lower-end hardware.
  - Custom scripts to handle service management.



## Kernel and Boot Options

- **Kernel**:
  - The Linux kernel is 6.15 for supporting maximum of hardware .

- **GRUB Configuration**:
  - To modify boot parameters, edit `/etc/default/grub` and update GRUB:
    ```bash
    sudo update-grub
    ```

## Custom Branding

- **Boot Splash Screen**:
  - Custom Dune OS boot splash screen.


## Reporting Issues

For bug reports or issues, open a ticket on the [GitHub repository](https://github.com/H3xKatana/DuneOS//issues).

