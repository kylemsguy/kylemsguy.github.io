---
layout: post
title: About Piracy
---
Ever since I became interested in computers and other electronic devices, I always wanted to do more with them, sometimes beyond what the manufacturer intended.
This wasn't a problem on computers, because there are absolutely no restrictions as to what you can install on them.
Need a word processor? Install Microsoft Office.
Want games? Go download some.
Want a new OS? Download it.
However, on every phone I dealt with predating the iPhone, I was always annoyed at the lack of useful apps on them, and the fact that it was extremely difficult, and sometimes impossible, to install more, whether it is to do with methods of installation (WAP only on older, lower-end phones), or to do with the fact that most of them were locked down.

Even when I got my first iPod (a nano 4G), I wished it had WiFi, and some proper apps instead of the limited selection of iPod games offered by Apple (not to be confused by the iPhone App Store). 
When I finally got my second-gen iPod touch, I felt like I was finally free. 
Full WiFi, Bluetooth support (which I didn't use much), and a huge selection of apps on the App Store. 
The best thing, however, was the fact that I could jailbreak it and get root access.
Now, not only did I have access to mountains of apps, I also had access to an even bigger mountain of apps, as well as modifications to the OS.
I could now run apps in the background, have quick toggles for WiFi and other things, homescreen wallpapers, and themes, just to name a few. (Keep in mind this was way back in iPhone OS 3.1.2!)
This continued after my upgrade to a 4th gen iPod touch, which gave me more power so that I could run more tweaks, although I did lose some freedom in that I could no longer change the boot logo (until GreenPois0n's animated boot screen), as well as not having a guaranteed untethered jailbreak. 

When I finally got a proper smartphone, I chose the Nexus 4. 
Now, I was truly free. 
Gone were the days of waiting for a new jailbreak to come out. 
Gone were the days of broken iTunes backups. 
With Android, I could just unlock the bootloader and flash SuperSU or install a custom ROM such as Cyanogenmod.
Even without doing so, I still had access to any apk that I wanted, instead of having to be restricted to Apple's walled garden.
For backups, I could just do a Nandroid or use Titanium Backup, without the problems of an iTunes backup + PkgBackup combo.
I could also finally do everything I could do on a full computer on my phone.
I had attempted to do this on my iPod touch, but it was still missing a few full-featured apps in order to be of much use, such as a proper web browser or a working C compiler.
Now I could freely install QPython from the Play Store, as well as Linux Deploy in order to get a full Linux distribution on my phone. 
Emulators no longer required jailbreaking, and I could swap out most parts of the OS even without root.
Custom ROMs also gave me features that I had to install tweaks for on my iOS devices.
I could replace the kernel with whatever I wanted.
I could roll my own ROM if I so desired.

The key to why I love Android is the freedom. 
The entire Android OS is open-source, so anyone who wants to can modify the OS.
It also allows the user to sideload apks, which means that alternative app stores can exist.
Now, I know that some phones out there are locked down almost as badly as iPhones, but they generally retain the ability to sideload apks.
However, recently there was a new [Anti-Piracy project](https://github.com/AlmightyMegadeth00/AntiPiracySupport) that some developers have started to incorporate into ROMs, such as Exodus or BrokenOS. 
What it does is look through your app's package identifier and compare it against a blacklist.
If the app is found to be on the blacklist, it automatically uninstalls the app from the device.
The developers behind the project claim that it's to help prevent piracy and malware.
While this sounds good on paper, I strongly oppose such a "feature" in the ROMs I use.

First of all, this project is ineffective at actually stopping piracy. 
Since it is merely a blacklist of package names, all anyone needs to do in order to circumvent it is to change the package name of the app.
This is extremely easy to do, and it only leads to a longer blacklist.
Another way is simply using root access in order to disable the relevant services.
As I understand it, the blacklist is not obfuscated on the device, so anyone with root could simply modify it.
Furthermore, the services do not block sideloading apks, which means that if the app has the same package identifier as a legitimate app, the service can do nothing to prevent their installation without preventing a user from installing the legitimate app.

This project also has features that are quite close to those in malware.
One of the key features of the services is that it removes apps that they think are either malware or for piracy.
However, by preventing the user from installing apps that they disagree with without giving the user to override is a feature found in many rogue antivirus programs, viruses, and other malware ([see here for an example](https://www.youtube.com/watch?v=wKzAqXkMH2w)).
Also, the project plans to [modify the HOSTS file](https://github.com/AlmightyMegadeth00/AntiPiracySupport/blob/4ea5a4c917389cc996c9c4ee19ccadde0f3f209d/src/AntiPiracyInstallReceiver.java) in order to prevent the user from accessing sites they believe focus on spreading malware or piracy.
The thing is, malware often modifies the HOSTS file in order to prevent the user from going to websites that it does not agree with, which in this case is sites where the user can get antivirus programs. 
