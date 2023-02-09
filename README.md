<h1  align="center">
  <img  src="https://avatars.githubusercontent.com/u/124920598?s=400&u=20b77b2b9fca9702860f9f66b129ee5dde165987&v=4"  alt="VERY COOL CAT">
  <p>meowc0ver</p>
</h1>
<h3  align="center">A iOS 15.0-16.3 WIP, (semi-)tethered checkm8 jailbreak.</h3>

# FAQ
Why do you use palera1n's app and sources?
We use the palera1n app and sources because they are already made for iOS 15 and 16 no point in really making another repo.

# How does it work?

I will put it in basic words first it puts patches on ur kernel first time u run it it boots a ramdisk that dumps stuff and creates a fakefs! (semi-tethered)

# Requirements

- A checkm8 vulnerable iOS device on iOS 15 or 16 (A8-A11)
	- The device must be on iOS 15.0-16.3
		- "dont ask for above stupid"
	-	If you want the device to be semi-tethered, **you will need 5-10GB of space** for the fakefs. This means that 16GB devices cannot be semi-tethered
	- ### A10 and A11 devices
		- If you are on A10(X), use [checkp4le](https://github.com/guacaplushy/checkp4le)
		- On A11, **you must disable your passcode while in the jailbroken state**.
		- On iOS 16 A11, if you EVER enabled a passcode on 16, you have to reset through the settings app/restore with a computer
		- use [FakePass](https://repo.alexia.lol/depictions/net.cadoth.fakepass) for fake passcode but it acts like its a real passcode

- A **USB-A to Lightning cable**
	- USB-C cables
		- yeah no usb-c never supported ever 

- A Linux or macOS computer
	- Python 3 must be installed.
	- This must be a **physical computer**. Virtual machines **do not work.**
	- amd cpus are dumb [with (likely) their USB controllers] that causes them to have a very low success rate with checkm8. It is not recommended that you use them with meowc0ver.
		- If your device does not successfully jailbreak, try a computer with an Intel or other CPU

# Warning

- if u screw up ur device ur on ur own
# How to use?

ez!
** NOTE: On linux usbmuxd has a issue and u need to do sudo systemctl stop usbmuxd && sudo usbmuxd -f -p in a second terminal and dont close that one while using meowc0ver **
Linux[
semi-tethered: sudo ./meowc0ver.sh --tweaks iosversion --semi-tethered
tethered: sudo ./meowc0ver.sh --tweaks iosversion

# Issues

**Please first check the [common issues](https://github.com/palera1n/palera1n/blob/main/COMMONISSUES.md) document.**

## Still need help?

Open a issue and we will help you asap!



**DO NOT** harass tweak devs if tweaks don't work. Refer to [here](https://github.com/itsnebulalol/ios15-tweaks) for compatiblity.



### Rootless

Repos need to be updated for rootless, here are some that work currently:

- [Mineek's repo](https://mineek.github.io/repo) contains rootless Procursus packages
- The official [palera1n repo](https://repo.palera.in) contains miscellaneous packages

If you want to make a rootless repo, use the official [palera1n repo](https://github.com/palera1n/repo) for reference. Every deb should use the `iphoneos-arm64` architecture, and *nothing* should be on the rootfs. Everything should be in /var/jb.

# Credits

- [Nathan](https://github.com/verygenericname)
	- The ramdisk that dumps blobs, copies files, and duplicates rootfs is a slimmed down version of [SSHRD_Script](https://github.com/verygenericname/SSHRD_Script)
	- For modified [restored_external](https://github.com/verygenericname/sshrd_SSHRD_Script)
	- Also helped Mineek getting the kernel up and running and with the patches
	- Helping with adding multiple device support
	- Fixing issues relating to camera.. etc by switching to fsboot
	- [iBoot64Patcher fork](https://github.com/verygenericname/iBoot64Patcher)
- [Mineek](https://github.com/mineek)
	- For the patching and booting commands
	- Adding tweak support
	- For patchfinders for RELEASE kernels
	- [Kernel15Patcher](https://github.com/mineek/PongoOS/tree/iOS15/checkra1n/Kernel15Patcher)
	- [Kernel64Patcher](https://github.com/mineek/Kernel64Patcher)
	- Work on jbinit, together with [Nick Chan](https://github.com/asdfugil)
- [Amy](https://github.com/elihwyma) for the [Pogo](https://github.com/elihwyma/Pogo) app
- [checkra1n](https://github.com/checkra1n) for the base of the kpf
- [nyuszika7h](https://github.com/nyuszika7h) for the script to help get into DFU
- [the Procursus Team](https://github.com/ProcursusTeam) for the amazing [bootstrap](https://github.com/ProcursusTeam/Procursus)
- [F121](https://github.com/F121Live) for helping test
- [m1sta](https://github.com/m1stadev) for [pyimg4](https://github.com/m1stadev/PyIMG4)
- [tihmstar](https://github.com/tihmstar) for [pzb](https://github.com/tihmstar/partialZipBrowser)/original [iBoot64Patcher](https://github.com/tihmstar/iBoot64Patcher)/original [liboffsetfinder64](https://github.com/tihmstar/liboffsetfinder64)/[img4tool](https://github.com/tihmstar/img4tool)
- [Tom](https://github.com/guacaplushy) for a couple patches and bugfixes
	- For maintaining [Kernel64Patcher](https://github.com/palera1n/Kernel64Patcher)
- [xerub](https://github.com/xerub) for [img4lib](https://github.com/xerub/img4lib) and [restored_external](https://github.com/xerub/sshrd) in the ramdisk
- [Cryptic](https://github.com/Cryptiiiic) for [iBoot64Patcher](https://github.com/Cryptiiiic/iBoot64Patcher) fork, and [liboffsetfinder64](https://github.com/Cryptiiiic/liboffsetfinder64) fork
- [libimobiledevice](https://github.com/libimobiledevice) for several tools used in this project (irecovery, ideviceenterrecovery etc), and [nikias](https://github.com/nikias) for keeping it up to date
- [Nick Chan](https://github.com/asdfugil) general help with patches and iBoot payload stuff
- [Dora](https://github.com/dora2-iOS) for iBoot payload and iBootpatcher2
- [Sam Bingner](https://github.com/sbingner) for [Substitute](https://github.com/sbingner/substitute)
- [Serena](https://github.com/SerenaKit) for helping with boot ramdisk.
