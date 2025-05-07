# WinDuck

![PLACEHOLDER](./docs/assets/Title-Screen.png)

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
