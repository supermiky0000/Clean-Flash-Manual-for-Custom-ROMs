# *General* clean-flash guide for custom ROMs installation
This is a guide designed for beginners, mainly for those who start from the stock ROM and want to install an [AOSP](https://source.android.com/)-based ROM. But it can be useful even to others.

a Clean Flash is when you format the data partition, this therefore means loss of your files.
There is only a few times you may need to clean flash:
- When going from one major version to another (like Android 13 to 14) and obv when downgrading too.
- When your device maintainer says it's required because of changes.
- Maybe other times like when u encounter bugs or errors

## Before starting (READ)

* You always have to follow the developers and device maintainers recommendations independently from this guide. The installation of Custom ROMs often depends from the device and you must have the specific files to install for yours.

* For installation of Custom ROMs you must have unlocked bootloader and it generally involves of void of warranty. Remember that not all devices have an unlockable bootloader. It's unlocking depends on the device and for it you must follow the manufacturer manual or a detailed tutorial on YouTube. You can also see your specific device forum on [XDA](https://xdaforums.com/).

* This guide skip the part of the data Backup. So if after the installation of a new ROM you want to restore all of your previous data (apps, photos...), you should consider to backup all your important files to your PC or in a cloud like Google Drive and Photos before starting. For this part I recommend you to follow a guide on Internet.

⚠ This guide should be safe but in case of bricked devices or bootloop I am NOT responsible. Follow always the manual of your specific device for OEM unlocking and be careful doing all this types of things.

## Guide
During this guide you should have a PC connected via USB because you will have to install all you need on it and then copy them in the Internal Storage/sdcard of the device. For this i recommend to create a folder on your desktop and install the files into it.

- For installation of Custom ROMs and not only (cause is a useful tool) you must have a Custom Recovery, for this guide i recommend [OrangeFox](https://orangefox.download/). Also for this part you have to follow the installation guide on the Recovery official page or on YouTube. After installation save a copy in the Internal Storage/sdcard because it'll come in handy in step 5.

Let's start:

1. Reboot to Custom Recovery (it depends on the device, usually is hold Power + Volume Down buttons) 
2. Copy the Firmware (if required) and Custom ROM to sdcard
3. Wipe Dalvik/ART, Cache, Metadata and Data partitions (do NOT reboot after this!)
4. Return to sdcard and flash first Firmware and then ROM
5. Flash the Recovery zip copy (it will probably reboot to recovery automatically, if not you have to do it manually)

~ If you have Gapps in your flashed ROM: Format Data and finally reboot to the new system

~ If you don't have Gapps built-in in the flashed ROM do these remaining steps:

⚠*This part is based on my experience on a Xiaomi/Redmi phone, so it will probably may vary on the device*

7. Format data and reboot to recovery
8. Go into "data" folder, create a folder named "media" then disable and reable MTP 
9. Now you have to copy RO2RW to the phone, you will see it in the created folder in the previous step, flash it and reboot to recovery
10. Now you can copy Gapps to sdcard and flash they
11. Format data and finally you can reboot to the new system

# Useful links
* [nikGapps](https://nikgapps.com/)
* RO2RW --> uploaded file or search on Internet
## Major Custom ROMs links
If you're a beginner and you do not know what to install, i recommend u to visit the websites of all ROMs, entering in your device maintainer Telegram group watching all the screenshots to see what you like and then decide which flash.
Remember to follow the maintainers' recommendations.
* [LineageOS](https://www.lineageos.org/)
* [crDroid](https://crdroid.net/)
* [Project Matrixx](https://www.projectmatrixx.org/)
* [RisingOS Revived](https://risingosrevived.tech/)
* [GrapheneOS](https://grapheneos.org/)
* [Derpfest](https://derpfest.org/)
* [EvolutionX](https://evolution-x.org/)

 if u want more search on Internet...
