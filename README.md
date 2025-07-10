# WinDuck

![sans](cool%20stuff/sans-_heya..png)

WinDuck is my complete guide on how to set up Windows 11 for as much performance and privacy without installing a single program.

The goal for this guide is to make *making Windows 11 usable* as easy and streamlined as possible, so anybody with any amount of experience can follow it :)

WinDuck does *not* contain any programs or scripts that I have made (trusting another stranger on the internet feels like a bad idea...), instead it uses [Winutil](https://github.com/ChrisTitusTech/winutil?tab=readme-ov-file) and [NextDNS](https://nextdns.io/), both of which do not install anything.

## Chapter 1: Winutil

Winutil is what is going to do 99% of making Windows stop using unnecessary amount of resources in the background, as well as disabling most telemetry, here's how we use it:

**1. Opening the terminal:**
To use Winutil we need to open the terminal (don't worry, it's easy):

   - Right click on the Windows button menu in the taskbar on the bottom of the screen
   - Click on "Terminal (Admin)"
   - Cick on "Yes" on the prompt that pops up

**1.1 Entering Winutil:**
Now that we have opened a terminal window, we need to paste the command that is going to run Winutil:

   - Copy the following block of text (if you want to double-check that the command is the official one, you can compare it on [Winutil's page](https://github.com/ChrisTitusTech/winutil?tab=readme-ov-file)):

```ps1
irm "https://christitus.com/win" | iex
```

   - Right click inside the black part of the terminal to paste it in
   - Press enter

**1.1 Using Winutil:**
Winutil is now open in 2 windows, one still in the terminal (which we can ignore) and one in a separate window

   - Click on "tweaks" on the top
   - Enable the following checkboxes:
- [x] Delete Temporary Files
- [x] Disable ConsumerFeatures
- [x] Disable Telemetry
- [x] Disable Activity History
- [x] Disable GameDVR (don't enable this one if you use the built in Game Bar recording, but I would recommend disabling it and using Steam's instead, it barely uses any resources)
- [x] Disable Homegroup
- [x] Disable Location Tracking
- [x] Disable Storage Sense
- [x] Disable Wifi-Sense
- [ ] Enable End Task With Right Click (Optional, it adds another button when you right click icons in the taskbar)
- [x] Run Disc Cleanup
- [x] Disale Powershell 7 Telemetry
- [x] Disable Recall
- [x] Set Services to Manual

Advanced section:
- [x] Disable Background Apps (if you use any wallpaper apps from the Microsoft Store that updates the wallpaper automatically, for example "Dynamic Theme", checking this option will prevent it from working in the background)
- [x] Disable Microsoft Copilot
- [x] Disable Intel MM (vPro LMS) (this option only works if you have an Intel CPU, skip it if you have AMD like me)
- [x] Remove ALL MS Store Apps (this option removes every app that has been installed through the Microsoft Store, it also removes the screenshot tool, so make sure that you don't have any data in any Store apps or games that you don't want to loose, you can install them and the screenshot tool (snipping tool) again after finishing this chapter)
- [x] Remove OneDrive (don't if you use OneDrive)

   - After checking all of these, press the "Run Tweaks" button in the bottom of the screen (you may have to expand the window or scroll down if you can't see it)

   - You will know that it is done when the terminal window tells you :)
     
**1.1 Using O&O Shutup:**
Now that we have used the main part of Winutil it is time to use the program built into Winutil, O&O Shutup.

   - In the same "tweaks" section, scroll to the bottom of the page (underneath the advanced section) and press "run O&O Shutup"
   - Now, it is really important to note that while I may not use any of the privacy-invasive features that we are going to disable, it is possible that you do, so read every single option that we are going to enable.
   - Enable the following options (so the slider on the right turns green): (there's a LOT, be prepared to take like 15 minutes to do these :))

Privacy

- [x] Disable and reset Advertising ID and info

- [x] Disable transmission of typing information

- [x] Disable suggestions in the timeline

- [x] Disable suggestions in Start

- [x] Disable tips, tricks, and suggestions when using Windows

- [x] Disable showing suggested content in the Settings app

- [x] Disable the possibility of suggesting to finish the setup of the device

- [ ] Disable app notifications (optional)

- [x] Disable access to local language for browsers

- [x] Disable text suggestions when typing on the software keyboard

- [x] Disable sending URLs from apps to Windows Store

Activity History and Clipboard

- [x] Disable storage of clipboard history (optional)

App Privacy

- [x] Disable app access to user account information

- [x] Disable Windows tracking of app starts

- [x] Disable app access to diagnostics information

- [x] Disable app access to device location

- [ ] Disable app access to camera (enabling this will disable your camera)

- [ ] Disable app access to microphone (enabling this will disable your microphone... I did NOT spend 30 minutes thinking my microphone was broken.)

- [x] Disable app access to use voice activation

- [x] Disable app access to use voice activation when device is locked

- [x] Disable the standard app for the headset button

- [x] Disable app access to notifications

- [x] Disable app access to movements

- [x] Disable app access to contacts

- [x] Disable app access to calendar

- [x] Disable app access to phone calls

- [x] Disable app access to call history

- [x] Disable app access to email

- [x] Disable app access to tasks

- [x] Disable app access to messages

- [x] Disable app access to radios

- [x] Disable app access to unpaired devices

- [x] Disable app access to documents

- [x] Disable app access to images

- [x] Disable app access to videos

- [x] Disable app access to the file system

- [x] Disable app access to wireless technology

- [x] Disable app access to eye tracking

- [x] Disable the ability for apps to take screenshots

- [x] Disable the ability for desktop apps to take screenshots

- [x] Disable the ability for apps to take screenshots without borders

- [x] Disable the ability for desktop apps to take screenshots without margins

- [x] Disable app access to music libraries

- [x] Disable app access to downloads folder

- [x] Prohibit apps from running in the background


Microsoft Edge (new version based on Chromium)
(note: I do not recommend using Edge.)

- [x] Disable tracking in the web

- [x] Disable check for saved payment methods by sites

- [x] Disable personalizing advertising, search, news and other services

- [x] Disable automatic completion of web addresses in address bar

- [x] Disable user feedback in toolbar

- [x] Disable storing and autocompleting of credit card data on websites

- [x] Disable form suggestions

- [x] Disable suggestions from local providers

- [x] Disable search and website suggestions

- [x] Disable shopping assistant in Microsoft Edge

- [x] Disable Edge bar

- [x] Disable Sidebar in Microsoft Edge

- [x] Disable the Microsoft Account Sign-In Button

- [x] Disable Enhanced Spell Checking

- [x] Disable use of web service to resolve navigation errors

- [x] Disable suggestion of similar sites when website cannot be found

- [x] Disable preload of pages for faster browsing and searching

- [x] Disable saving passwords for websites

- [x] Disable site safety services for more information about a visited website (if you NEED to use Edge... don't enable this.)

- [x] Disable SmartScreen Filter (if you NEED to use Edge... don't enable this.)

- [x] Disable typosquatting checker for site addresses (if you NEED to use Edge... don't enable this)

Microsoft Edge (legacy version)
(again, please use another browser)

- [x] Disable tracking in the web

- [x] Disable page prediction

- [x] Disable search and website suggestions

- [x] Disable Cortana in Microsoft Edge

- [x] Disable showing search history

- [x] Disable form suggestions

- [x] Disable sites saving protected media licenses on my device

- [x] Do not optimize web search results on the task bar for screen reader

- [x] Disable SmartScreen Filter

Synchronization of Windows Settings

- [x] Disable synchronization of all settings

- [x] Disable synchronization of design settings

- [x] Disable synchronization of browser settings

- [x] Disable synchronization of credentials (passwords)

- [x] Disable synchronization of language settings

- [x] Disable synchronization of accessibility settings

- [x] Disable synchronization of advanced Windows settings

- [x] Cortana (Personal Assistant)

- [x] Disable and reset Cortana

- [x] Disable Input Personalization

- [x] Windows Al

- [x] Disable the Windows Copilot

- [x] Disable the Copilot button from the taskbar

- [x] Disable Windows Copilot+ Recall

User Behavior

- [x] Disable the use of diagnostic data for a tailor-made user experience

Windows Explorer


- [x] Disable occassionally showing app suggestions in Start menu

- [x] Do not show recently opened items in Jump Lists on "Start" or the taskbar

- [x] Disable ads in Windows Explorer/OneDrive

Lock Screen

- [x] Disable Windows Spotlight

- [x] Disable fun facts, tips, tricks, and more on your lock screen

- [x] Disable notifications on lock screen

Mobile Devices

- [x] Disable access to mobile devices

- [x] Disable Phone Link app

- [x] Disable showing suggestions for using mobile devices with Windows

Search

- [x] Disable search with Al in search box

- [x] Disable extension of Windows search with Bing

Taskbar

- [x] Disable People icon in the taskbar

- [x] Disable search box in task bar

- [x] Disable "Meet now" in the task bar

- [x] Disable widgets in Windows Explorer

Miscellaneous

- [x] Disable feedback reminders

- [x] Disable automatic installation of recommended Windows Store Apps

- [x] Disable tips, tricks, and suggestions while using Windows

- [x] Disable Windows Media Player Diagnostics

- [x] Disable the desktop icon for information on "Windows Spotlight"

Privacy

- [x] Disable sharing of handwriting data

- [x] Disable sharing of handwriting error reports

- [x] Disable Inventory Collector

- [x] Disable camera in logon screen

- [x] Disable and reset Advertising ID and info for the machine

- [x] Disable advertisements via Bluetooth

- [x] Disable the Windows Customer Experience Improvement Program

- [x] Disable backup of text messages into the cloud

- [x] Disable Windows Error Reporting

- [x] Disable biometrical features

Activity History and Clipboard

- [x] Disable recordings of user activity

- [x] Disable storing users' activity history

- [x] Disable the submission of user activities to Microsoft

- [x] Disable storage of clipboard history for whole machine

- [x] Disable the transfer of the clipboard to other devices via the cloud

App Privacy

- [x] Disable app access to user account information

- [x] Disable app access to diagnostics information

- [x] Disable app access to device location

- [ ] Disable app access to camera

- [ ] Disable app access to microphone

- [x] Disable app access to notifications

- [x] Disable app access to motion

- [x] Disable app access to contacts

- [x] Disable app access to calendar

- [x] Disable app access to phone calls

- [x] Disable app access to call history

- [x] Disable app access to email

- [x] Disable app access to tasks

- [x] Disable app access to messages

- [x] Disable app access to radios

- [x] Disable app access to unpaired devices

- [x] Disable app access to documents

- [x] Disable app access to images

- [x] Disable app access to videos

- [x] Disable app access to the file system

- [x] Disable app access to wireless equipment

- [x] Disable app access to eye tracking

- [x] Disable the ability for apps to take screenshots

- [x] Disable the ability for apps to take screenshots without borders

- [x] Disable app access to music libraries

- [x] Disable app access to downloads folder

Security

- [x] Disable password reveal button

- [x] Disable user steps recorder

- [x] Disable telemetry

- [ ] Disable Internet access of Windows Media Digital Rights Management (DRM)

Microsoft Edge (new version based on Chromium)

- [x] Disable tracking in the web

- [x] Disable check for saved payment methods by sites

- [x] Disable personalizing advertising, search, news and other services

- [x] Disable automatic completion of web addresses in address bar

- [x] Disable user feedback in toolbar

- [x] Disable storing and autocompleting of credit card data on websites

- [x] Disable form suggestions

- [x] Disable suggestions from local providers

- [x] Disable search and website suggestions

- [x] Disable shopping assistant in Microsoft Edge

- [x] Disable Edge bar

- [x] Disable Sidebar in Microsoft Edge

- [x] Disable the Microsoft Account Sign-In Button

- [x] Disable Enhanced Spell Checking

- [x] Disable use of web service to resolve navigation errors

- [x] Disable suggestion of similar sites when website cannot be found

- [x] Disable preload of pages for faster browsing and searching

- [x] Disable saving passwords for websites

- [x] Disable site safety services for more information about a visited website

- [x] Disable automatic redirection from Internet Explorer to Microsoft Edge

- [ ] Disable SmartScreen Filter

- [ ] Disable typosquatting checker for site addresses

Microsoft Edge (legacy version)

- [x] Disable automatic completion of web addresses in address bar

- [x] Disable user feedback in toolbar

- [x] Disable storing and autocompleting of credit card data on websites

- [x] Disable Microsoft Edge launch in the background

- [x] Disable loading the start and new tab pages in the background

- [x] Cortana (Personal Assistant)

- [x] Disable online speech recognition

- [x] Cortana and search are disallowed to use location

- [x] Disable web search from Windows Desktop Search

- [x] Disable display web results in Search

- [x] Disable download and updates of speech recognition and speech synthesis models

- [x] Disable cloud search

- [x] Disable Cortana above lock screen

- [x] Disable the search highlights in the taskbar

Windows Al

- [x] Disable the Windows Copilot

- [x] Disable Windows Copilot+ Recall

Location Services

- [x] Disable functionality to locate the system

- [x] Disable scripting functionality to locate the system

- [x] Disable sensors for locating the system and its orientation

- [x] Disable Windows Geolocation Service

User Behavior

- [x] Disable application telemetry

- [x] Disable diagnostic data from customizing user experiences for whole machine

- [x] Disable diagnostic log collection

- [x] Disable downloading of OneSettings configuration settings

Windows Update

- [x] Disable Windows Update via peer-to-peer (this will NOT disable updates)- [x] 

- [x] Disable updates to the speech recognition and speech synthesis modules.

- [x] Activate deferring of upgrades

- [x] Disable automatic downloading manufacturers' apps and icons for devices

- [ ] Disable automatic driver updates through Windows Update

- [ ] Disable automatic app updates through Windows Update

- [ ] Disable Windows dynamic configuration and update rollouts

- [ ] Disable automatic Windows Updates

- [x] Disable Windows Updates for other products (e.g. Microsoft Office)

Windows Explorer

- [x] Disable OneDrive access to network before login

- [x] Disable Microsoft OneDrive (if you don't use OneDrive... but I recommend using something else, or OneDrive in the web browser.)

Microsoft Defender and Microsoft SpyNet

- [x] Disable Microsoft SpyNet membership

- [x] Disable submitting data samples to Microsoft

- [x] Disable reporting of malware infection information

Mobile Devices

- [x] Disable connecting the PC to mobile devices

Taskbar

- [x] Disable "Meet now" in the task bar

- [x] Disable news and interests in the task bar

Miscellaneous

- [x] Disable feedback reminders

- [x] Disable remote assistance connections to this computer

- [x] Disable remote connections to this computer (Third party apps like Steam Link still work with this disabled.)

- [ ] Disable Key Management Service Online Activation

- [x] Disable automatic download and update of map data

- [x] Disable unsolicited network traffic on the offline maps settings page

- [ ] Disable Network Connectivity Status Indicator

## Chapter 2: NextDNS

Now we have disabled as much garbage running in the background as we possibly can, however, Windows will STILL "phone home", which could be invasive to your privacy. To mitigate this, we will set up NextDNS.

**2.1 Creating NextDNS account and changing DNS:**

   - Go to the [official NextDNS website](https://nextdns.io/)
   - Click "my nextdns io" on the top
   - Click sign up and sign up
   - Scroll down to "setup guide", click Wndows and follow the setup guide (they probably explain it better than me lol)

**2.2 Configuring NextDNS:**
NextDNS has very weak tracker-blocking by default, but it's super easy to make it very good:

   - Click "Security"
   - Enable as much as you want here :) I enabled all of the options (except Block Top-Level Domains (TLDs))
   - Click "Privacy"
   - Click "Add a Blocklist"
   - Search for "HaGeZi - Multi ULTIMATE" and click add, then close the blocklist window
   - Scroll down to "Native Tracking Protection", click "add" and select Windows
   - Scroll down and enable "Block Disguised Third-Party Trackers"
   - Scroll to the top again and press "Settings"
   - Enable "Anonymized EDNS Client Subnet" and "Cache Boost"
   - NextDNS is now fully configured!!!

**2.3 Blocking... EVERY SINGLE MICROSOFT CONNECTION??? (optional):**
Or is it.
NextDNS will now block every tracking connection that Wndows does, however, there are still Microsoft services that Windows connects to, which can be considered privacy invasive. 
This step is pretty extreme and optional, but if you are like me and dont use and Microsoft services anyway (except Windows update), then why not.

   - Click  "Allowlist"
   - Enter [every single domain separately](https://github.com/Gagnefs/WinDuck/blob/main/cool%20stuff/NextDNS%20Allowlist) (these are all required for Windows Update to work)
   - Click "Denylist"
   - Enter [Every single domain separately](https://github.com/Gagnefs/WinDuck/blob/main/cool%20stuff/NextDNS%20Denylist) (I know there's a lot. Blame Microsoft for all of this)
   - Actually done!!! Reboot to see everything being blocked in "Logs". This will also block trackers from other apps as well.

**2.4 Setting the browser to not use NextDNS:**

NextDNS has a limit on how many free queries you get per month. The limit is pretty high for 1 device, but this combined with the fact that the Hagezi list is very aggressive and may break some webstes, you may want to set up DNS over HTTPS in your browser.


   - If you aren't already using Firefox, install it.
   - Click the menu button in the top right
   - Click "Settings"
   - Click "Privacy & Security" and scroll to the bottom
   - Click "Max Protection" and select either CloudFlare or NextDNS (it does not use the same NextDNS account you made)
