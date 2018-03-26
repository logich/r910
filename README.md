Specifications:
- Battery Life: 12 hrs usage / 27 hrs standby
- Number of Connected Devices: 10 Wi-Fi
- Networks supported:
- LTE Bands: 25, 26, 41 (aka "Sprint Spark") - hardware also supports 2, 4, 5, 12
- 3G: Yes
- LTE-Advanced Carrier Aggregation: Yes
- LTE Performance Category: Category 4
- (Max Theoretical Speed: 150Mbps Down / 50Mbps Up)
- Cellular Antenna Ports: None
- Wi-Fi Technology / Frequencies: 802.11 b/g/n - 2.4GHz , 802.11ac - 5GHz
- Dimensions:    3.46" x 2.62" x 0.47" /  3.5 oz

Antenna Notes:
- Oficially no antenna jacks.
- R910 has small black stickers covering 6 TS9 female connectors. 
- These are around the perimeter of the device, not under the battery or label. ![device diagram](/device-diagram.png)
- the plastic surround of the device contains small antennas that are connected to pads next to these ports.
- ports are labeled in pairs: 1708 MAIN, 1708 DIV, B41 MAIN, B41 DIV
- Plugging an antenna into two of the matched pairs does increase the signal (RSSI and RSRQ)
- View signal values at http://192.168.128.1/hidden/debug-lte_engineering.html
- To make connections with the TS9, I needed to drill out plastic surrounds with 1/4 inch drill.
- Placing a $20 panel antenna on an old satelite disk and directing this at the tower increase signal strength and speed.

Tethering Notes:
- Set the USB mode for tethering under http://192.168.128.1/webpst/usb_mode.html and change to mode "RNDIS + DIAG + ADB [Android]"
- This makes it look like a phone for tethering versus a dumb modem or usb stick.
- Connect this to a super cheap GL.iNet mini router and configure it for tethering: https://www.gl-inet.com/docs/mini/3g4g/#phone-modem-tethering
- Connect the upstream router to the GL.iNet LAN port and configure it to do DHCP
- This will get an IP from the r910 directly versus double NAT.
- Then MultiWAN can be configured on the main router.

Sources:

https://buildyourownantenna.blogspot.com/2014/07/guide-to-antenna-cables-and-connectors.html

http://specialistantennas.blogspot.com/2013/05/the-10-most-comon-rf-coaxial-connectors.html

Device operates within approved frequencies overlapping with the following cellular bands:
 LTE 255,Unlicensed NII-3 DOWN | LTE 46,TD Unlicensed DOWN |
https://fccid.io/XHG-R910
https://fccid.io/png.php?id=3539957&page=6

https://www.calyxinstitute.org/sites/all/documents/hardware/Sprint_R910_UserGuide_English.pdf

https://www.reddit.com/r/Calyx/comments/7ofbjb/r910_sucks/dupqvn3/?context=1

Where to see LTE details on the R910:
http://192.168.128.1/hidden/debug-lte_engineering.html

Where to change USB mode for tethering:
http://192.168.128.1/webpst/usb_mode.html
change to mode "RNDIS + DIAG + ADB [Android]"

http://fweb.wallawalla.edu/~frohro//Airport/Primestar/Primestar.html

http://hpanswers.blogspot.com/2014/07/differnce-between-crc9-and-ts9-antenna.html

https://www.sprint.com/en/shop/hotspots/franklin-r910-mobile-hotspot.html

https://www.rvmobileinternet.com/review-center/sprint-r910-franklin-wireless/



