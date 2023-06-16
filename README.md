# Raspberry Pi Screen Setup

## Required Tools 
- USB Mouse
- USB Keyboard
- SD Card Reader
- Laptop
- Full Raspberry Pi Kit

## Copying ISO To New SD Card


## Set Up Web Browser Autostart
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
|Display|URL|
|---|---|
|THD-G1191-5|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1191_5|
|THD-G1216‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1216_1|
|THD-G1221‐A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1221_a|
|THD-G1225‐A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1225_a|
|THD-G1227‐A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1227_a|
|THD-G1191‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1191_1|
|THD-G1191‐6|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1191_6|
|THD-G1215‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1215_1|
|THD-G1216‐2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1216_2|
|THD-G1222‐A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1222_a|
|THD-G1226‐A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1226_a|
|THD-G1192‐3|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1192_3|
|THD-G1215‐3|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1215_3|
|THD-G1218‐A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1218_a|
|THD-G1224‐A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1224_a|
|THD-G1191‐4|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1191_4|
|THD-G1220‐A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1220_a|
|THD-G1192‐2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1192_2|
|THD-G1192‐3|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1192_3|
|THD-G1192‐9|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1192_9|
|THD-G1209‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1209_1|
|THD-G1210‐3|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1210_3|
|THD-G1211‐2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1211_2|
|THD-G1211‐6|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1211_6|
|THD-G1212‐3|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1212_3|
|THD-G1213‐4|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1213_4|
|THD-G1214‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1214_1|
|THD-G1214‐5|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1214_5|
|THD-G1192‐4|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1192_4|
|THD-G1192‐8|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1192_8|
|THD-G1209‐2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1209_2|
|THD-G1210‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1210_1|
|THD-G1210‐7|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1210_7|
|THD-G1211‐3|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1211_3|
|THD-G1212‐4|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1212_4|
|THD-G1213‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1213_1|
|THD-G1213‐5|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1213_5|
|THD-G1214‐2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1214_2|
|THD-G1214‐6|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1214_6|
|THD-G1211‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1211_1|
|THD-G1211‐4|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1211_4|
|THD-G1211‐5|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1211_5|
|THD-G1212‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1212_1|
|THD-G1212‐5|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1212_5|
|THD-G1213‐2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1213_2|
|THD-G1213‐3|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1213_3|
|THD-G1213‐6|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1213_6|
|THD-G1214‐3|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1214_3|
|THD-G1214‐4|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1214_4|
|THD-G1228‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1228_1|
|THD-G1193‐5|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1193_5|
|THD-G1193‐7A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1193_7a|
|THD-G1196‐3|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1196_3|
|THD-G1197‐2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1197_2|
|THD-G1203‐A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1203_a|
|THD-G1206‐2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1206_2|
|THD-G1207‐2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1207_2|
|THD-G1208‐3|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1208_3|
|THD-G1193‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1193_1|
|THD-G1193‐6|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1193_6|
|THD-G1196‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1196_1|
|THD-G1198‐A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1198_a|
|THD-G1204‐A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1204_a|
|THD-G1206‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1206_1|
|THD-G1207‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1207_1|
|THD-G1208‐1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1208_1|
|THD-G1208‐2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1208_2|
|THD-G1193-4|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1193_4|
|THD-G1193-8A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1193_8a|
|THD-G1196-2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1196_2|
|THD-G1197-1|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1197_1|
|THD-G1199-A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1199_a|
|THD-G1200-A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1200_a|
|THD-G1201-A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1201_a|
|THD-G1202-A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1202_a|
|THD-G1205-A|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1205_a|
|THD-G1228-2|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1228_2|
|THD-G1228-4|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1228_4|
|THD-G1228-3|http://ignition.research.pemo/data/perspective/client/CVIPSS/aru/g/thd_g1228_3|
