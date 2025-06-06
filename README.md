# OpenCore Setup for ThinkPad E550

This setup is meant ONLY For this model, may work on other thinkpads, currently only tested on this
Designed for Monterey Only, you can try older, but Monterey is latest it supports (Ventura was too much pain)

## Hardware this was made for

Was made for 2core haswell i3 (1,7 GHz Dual-Core Intel Core i3)
Was made for Intel HD 4400 graphics, but any should work if you set it properly with opencore
Intel wifi card (wifi actually working)
Sound card should be cx20751/2 (the ssdt is placed there to support this)
I use 8gbs ram, shouldnt be an issue to have less or more (use atleast 4gb, system on itself uses like 1,5gb's ram)

## Setup

1. Download Monterey with macrecovery in OpenCore repository
2. With Macserial or GenSMBIOS to Give yourself serial with macbookpro 11,4 (crucial, as all is setted for this special smbios, dont worry, it works)
3. In the ROM, use your ethernet mac address (crucial for getting iservices working)

### post install

1. Create Apple ID (yes it also works fully)
2. Install Amphetamine
3. Install brew
4. With brew install python3 and python3-pip
5. after that, build your ProperTree as App and move it to Applications
6. Reccomend installing hackintool for debuging purposes
7. IF YOU HAVE IPHONE, TURN ON MESSAGE SHARING AFTER ADDING YOUR MAC TO APPLE ID
8. For iMessages to get working, first Open IMessages in terminal, and call apple support with the info that you got a popup saying that it says to call apple support and give them this code (shows in terminal, if not, try first to login, should kick you out with the code in terminal). You gotta play very much clueless or they can find out you use hackintosh and block your apple id. When they ask for serial, mention its "Bough off some marketplace or bazar and may or may not be repaired. (For me, they made the serial from error to valid, so it can also happen to you, please do not set purchase date, you dont really need it)

## Issues

Bluetooth is kinda quirky (not really sure, my antenas are dead)
Airdrop WONT work unless on apple broadcom (havent tried yet)
Sleep issues (should sleep without crashing, but disables Backlight + Sound buttons, sometimes battery readouts, reccomend installing amphetamine and leaving it on pernamently for now)
USB Accessory needs power issues (mapping is done lightly (Very much thanks to the firmware developeres for putting devices under first 15))

## Whats working?

Everything not specified in the Issues

## Todo's

Fix The sleep (could or could not work already, its kinda quirky)
Fix usb accessory needs power (usb map issue maybe?)

## Problem?

Either try to fix it first yourself with opencore wiki, or create an issue, if you have fixed anything in Issues, please pull request 🙏
