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




