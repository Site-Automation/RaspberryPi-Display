# Raspberry Pi Screen Setup

## Required Tools 
---
- USB Mouse
- USB Keyboard
- SD Card Reader
- Laptop
- Full Raspberry Pi Kit

## Copying ISO To New SD Card
---


## Set Up Web Browser Autostart
---
Open a terminal and enter the following command to navigate to the autostart directory </br>
`cd .config/autostart` </br>
Edit the startup script by entering the following command; the file should be empty </br>
`nano kiosk.desktop` </br>
Uncomment the last line and replace `{url}` with the provided url for the corresponding display. The resulting code should look like the following: </br>
```
[Desktop Entry]
Type=Application
Name=Kiosk
Exec=/usr/bin/bash chromium-browser --kiosk {url}
```
Where {url} is replaced with the corresponding url.

Finally hit `ctl+x` to exit and `y` to save upon exit. Reboot the Raspberry Pi to check if the screen automatically boots to the correct web page, be sure the page is shown in kisok mode (no tab control and no os header on top). 

## URL Mapping
