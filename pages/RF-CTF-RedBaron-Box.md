## RedBaron's RF CTF Box

![RedBaron RF CTF Box](https://github.com/rfhs/rfhs-wiki/blob/master/files/images/whatsinthebox/RedBaron-Box.jpg)

## Inventory
* Intel Nuc
* Slimq 240W Power Supply
* Nuand bladeRF 2.0 micro xA9
  * Nuand bladeRF CNC Aluminum Case
  * Nuand BT-100 Bias-tee Power Amplifier
  * SCH-32 antenna
* Ettus USRP B200
  * Linx 433 MHz antenna
* IEEE 802.15.4 Challenge
  * 2x Arduino Uno with XBee shields
* 6LoWPAN Challenge
  * 2x Raspberry Pi with Openlabs 802.15.4 modules
* Unication FLEX Pager
* Unication POCSAG Pager

## What Does This Box Do?
This box runs the IEEE 802.15.4 challenges, the 6LoWPAN challenges, and Software Defined Radio (SDR) challenges that are experimental or not yet integrated into [challengectl](https://github.com/rfhs/challengectl). The Unication pagers are the receivers for the POCSAG TX and FLEX TX challenges, where RF CTF contestants need to send a message to the pagers using the POCSAG or FLEX pager protocols. The Intel Nuc runs [Pentoo](https://pentoo.ch/) and most commonly uses [GNU Radio](https://www.gnuradio.org/) and various GNU Radio modules to transmit the experimental challenges using the USRP B200 and/or the bladeRF 2.0 micro.

## Other information about the box
The panel in the lid of the case that the Raspberry Pis, Arduinos, and Pagers are mounted to is the Pelican EZ-Click&trade; MOLLE Panel. Each of those devices are mounted to the panel with velcro, and the straps that the pagers are clipped to serve double duty to secure a small case to the lid while transporting the case.

The aluminum panel in the bottom of the case is a Pelican 1510 Interior Sub-Panel from DataPro. The rear panel with power, network, and USB inlets was also made by DataPro, to RedBaron's specifications.

The name plate on the case started as a blank anodized aluminum name plate from DataPro, and was laser engraved by RedBaron with the RFHS logo, his handle, and a QR code for [https://rfhackers.com](https://rfhackers.com).