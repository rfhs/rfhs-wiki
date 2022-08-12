# RF CTF RFID NFC Challenges
This should be considered a general list with general information for in person RFID/NFC challenges.

All challenges are subject to change and may be available only if the code or equipment is working.
Please check with staff if you have any questions.

## In Person
All challenges are currently only available in person.  We hope to add virtual RFID/NFC challenges in the future.  Good luck!

## Tools
For these challenges you should bring tools for Low Frequency (LF), High Frequency (HF), and Ultra High Frequency (UHF) RFID.

### LF and HF
Proxmark3 - The Swiss Army Knife of RFID research, paired with the bleeding edge RRG/Iceman firmware & client

### UHF
Note: Most UHF readers are also capable of writing.

Some good handheld options with internal antennas are the Zebra MC3190-Z which can be found on eBay for ($80-$130), or a more modern Zebra TC20 wth RFD2000 sled. There are also some untested generic UHF RFID Sleds available from various online retailers
- https://www.zebra.com/us/en/support-downloads/rfid/rfid-handhelds/mc3190-z.html
- https://www.zebra.com/us/en/products/rfid/rfid-handhelds/rfd2000.html
- https://www.zebra.com/us/en/support-downloads/mobile-computers/handheld/tc20.html

Industrial fixed position readers from Impinj or Alien also work well with external antennas.

UHF RFID Modules are another potential option for integrating into your kit:
- https://www.sparkfun.com/products/14066
- https://shop.m5stack.com/products/uhf-rfid-unit-jrd-4035

Additionally there are some (currently untested) SDR based UHF RFID reader implementations:
- https://github.com/AdamLaurie/Gen2-UHF-RFID-Reader

# Challenges

## RFHS_RFID_PACS_X
### Physical
This time we didn't just bring a building in a box, we brought the parking lot as well. There will be a range of different credential technlogies (LF, HF, UHF), some you can get your hands on, and some placed out of reach requiring creativity and determination.  You will need to use a variety of tools (including a UHF RFID Reader/Writer) and techniques to interact with our PACS (Physical Access Control System).

5 sets of cards will be at the front table

other sets will be on contestant tables


THIS IS A LEARNING JOURNEY

### Flags
There are 15 flags or more depends on the pain we want to deploy of varying difficulty that will be displayed on-screen upon successful presentation to the correct reader.

### Hint
<details>
  <summary>Click here to see hint</summary>
The Road to El Dorado is paved with misconfigurations, but the gate is protected with a PIN, demonstrate mastery over the bits and input a valid PIN on readers without a PIN pad.
</details>

## RFHS_RFID_UHF_X
### Physical
Find the UHF tag with EPC 554846435446 and explore it

### Flag
A flag will be revealed to you upon success of this challenge

### Hint
<details>
  <summary>Click here to see hint</summary>
The first 32 bits of the TID are: `E2801140`
</details>

## RFHS_RFID_UHF_Hunt_n (Tentative will announce via comms channels)
### Physical
DEF CON is a warehouse and we need your help to take inventory. UHF RFID tags will be everywhere, and details will be announced on Day 1 to start your search.

### Flag
Flags will be stored in the user memory of matching tags, submit flags as announced.


## Wireless OSDP

This is a wild one, this will be hard

you will need to relay from one place to another

attacks against the wireless interface is in play to inject data

This is new bring your A game even googling will be hard
