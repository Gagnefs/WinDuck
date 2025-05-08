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
