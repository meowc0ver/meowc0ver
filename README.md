<h1  align="center">
  <img  src="https://avatars.githubusercontent.com/u/111437912?v=4"  alt="VERY COOL CAT">
  <p>meowra1n</p>
</h1>
<h3  align="center">the cutest jailbreak ever!</h3>


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
	- amd cpus are dumb [with (likely) their USB controllers] that causes them to have a very low success rate with checkm8. It is not recommended that you use them with meowra1n.
		- If your device does not successfully jailbreak, try a computer with an Intel or other CPU

# Warning

- if u screw up ur device ur on ur own
# How to use?


**NOTE: On linux usbmuxd has a issue and u need to do sudo systemctl stop usbmuxd && sudo usbmuxd -f -p in a second terminal and dont close that one while using meowra1n**
<br>
Linux
<br>
semi-tethered: sudo ./meowra1n.sh --tweaks iosversion --semi-tethered
<br>
tethered: sudo ./meowra1n.sh --tweaks iosversion

mac is same but without sudo



## Need help?

Open a issue and we will help you asap!



**DO NOT** harass tweak devs if tweaks don't work. Refer to [here](https://github.com/itsnebulalol/ios15-tweaks) for compatiblity.




