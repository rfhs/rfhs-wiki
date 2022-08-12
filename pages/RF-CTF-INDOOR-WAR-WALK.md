# RFCTF INDOOR WAR WALK the A/C edition

## Info

The Indoor War Walk is new event that are doing with collaboration of the RF Hackers Sanctuary and [Wigle.net](https://wigle.net) team. Contestants walk, dance, and skateboard all while mapping access points in VEGAS like yes in the state of Nevada.  This will be the largest indoor Wireless Survey with location data.

This will be scored differently than the WWWD. All foxes are behind locked dorrs inside with in the following grid

![IDWW](/files/images/indoorwarwalk/thegrid.png)

There are 10 foxes within this grid. You will be scored on how many foxes you find out of 10.  The fox SSID and BSSID will not be provided. This is a blind coverage.  The more complete the more foxes.  Your foxes will be scored in wigle. All uploads MUST have location data to be scored in Wigle.

## Hardware
The are two main categories for hardware, computers and Android devices. Each have their pros and cons, but an Android device and the Wigle app will most likely be the easiest to start with. Possibly no cost if you already have the device.

### Android devices
#### Wigle App
Getting started using the Wigle app couldn't be easier. Download the app, [disable wifi scan throttling](https://pzoleeblogen.wordpress.com/2019/09/04/android-10-improve-wifi-scan-accuracy-disable-throttling/), sign into the app, and you're set to wardrive. **Note: Android 9** should be avoided as there is no way to disable wifi scan throttling. More app related information can be found in the [app FAQ](https://wigle.net/wiwiwa-faq).

Wigle app download - [[Play Store]](https://play.google.com/store/apps/details?id=net.wigle.wigleandroid) [[Raw APK]](https://github.com/wiglenet/wigle-wifi-wardriving/blob/master/dist/release/wiglewifiwardriving-release.apk) [[F-Droid]](https://f-droid.org/en/packages/net.wigle.wigleandroid/)

#### Misc
- [Automate the Wigle app with broadcast intents](https://wigle.net/phpbb/viewtopic.php?t=2707)

---

### Computers (laptops, SBC, etc.)
#### Kismet
Kismet allows for more options and flexibility with hardware. For example, you can choose which [wifi adapters](https://www.kismetwireless.net/docs/readme/datasources_wifi/#supported-hardware) and how many you want to use. There is more setup involved than using the Wigle app, but it's not difficult when using the [Kismet package repositories](https://www.kismetwireless.net/docs/readme/packages/) and reading through the [config files documentation](https://www.kismetwireless.net/docs/readme/config_files/).

[Wardriving mode](https://www.kismetwireless.net/docs/readme/wardriving/) is a configuration overlay that optimizes settings for wardriving specifically, and only keeps the required data needed for a Wigle submission. Using wardriving mode can greatly reduce the amount of load on your computer. It also logs networks straight to a Wigle compatible csv file, no post processing required.

When using Raspberry Pi, a Raspberry Pi 4 is recommended due to having much better performance than its predecessors. It's not that it won't work, but it may not work well.

#### GPS
Portable Wigle devices have a location without GPS feature (you are welcome and good luck this is your only warning)
You will need a GPS source to feed your location to Kismet. [Wytshadow's video](https://www.youtube.com/watch?v=2h8H3XEgWvw) may help you decide which is best for you. If you can't get your GPS to lock, or it loses its lock, you have [USB 3 interference](https://www.usb.org/sites/default/files/327216.pdf). USB 3 interference largely affects devices at 2.4GHz (which will also inhibit you from hearing devices you're attempting to detect), but depending on the level it could affect GPS receivers as well.
- [GM-3N](https://www.amazon.com/GM-3N-professional-Receiver-adjustable-GPS/dp/B07BPM9C1Q)
- [GlobalSat BU-353-S4](https://www.amazon.com/GlobalSat-BU-353-S4-Receiver-Black-Improved-New/dp/B098L799NH)
- [VK-172 GPS/GLONASS](https://www.amazon.com/Diymall-G-Mouse-Glonass-Raspberry-Aviation/dp/B00NWEEWW8/)

If you don't can't procure a hardware GPS for whatever reason, you can use one of the following apps which should allow you to connect to GPSD on your host hardware.
- [Share GPS - Android](https://play.google.com/store/apps/details?id=com.jillybunch.shareGPS)
- [GPSd Client - Android](https://play.google.com/store/apps/details?id=io.github.tiagoshibata.gpsdclient)
- [NMEA Gps - iOS](https://apps.apple.com/us/app/nmea-gps/id590868529)

#### Misc
- [Kismet Discord](https://discord.gg/5N4ME9a)

- [USB 3 interference](https://www.usb.org/sites/default/files/327216.pdf)

- [upload2wigle script](https://github.com/elkentaro/upload2wigle)

- [Def Con 29 WWWD rigs](DEFCON-29-WWWD-RIGS.md)

---

### Other
[Jhewitt ESP32 Wardriver project](https://wardriver.uk) A neat project that uses (2) ESP microcontrollers and off the shelf components to create a capable mini 2.4GHz stumbling rig.

---

## Mapping
It's important to know where you've been and where you want to go. Planning your route ahead of time is helpful and one less thing to worry about when you're driving.

### Google Maps
[Google Maps](https://www.google.com/maps/d/u/0/) allows you to easily create a map with your quadrant boundaries, and markers for specific areas you may want to give more attention to. It can be opened on your mobile device to provide directions to markers, and view of your current location to ensure you're in your quadrant.

![gmaps](https://raw.githubusercontent.com/rfhs/rfhs-wiki/master/files/images/wwwd/gmaps.jpg)


### Wigle app
The Wigle app also has a feature that will allow track where you have been.
- "Display routes for execution" will overlay the route you have taken since the app was launched.
- "Log routes for execution" will log your route, and can be viewed and exported as a GPX file via the Database page.

![wigleRoute](https://raw.githubusercontent.com/rfhs/rfhs-wiki/master/files/images/wwwd/wigleRoute.jpg)
![savedRoute](https://raw.githubusercontent.com/rfhs/rfhs-wiki/master/files/images/wwwd/savedRoute.jpg)




## **Always be capturing, upload often. Mo Radios Mo Packets.**
