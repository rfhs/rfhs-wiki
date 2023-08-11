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

Most UHF readers are also capable of writing. 

Some good handheld options with internal antennas are the Zebra MC3190-Z which can be found on eBay for ($80-$130), or a more modern Zebra TC20 wth RFD2000 sled.
- https://www.zebra.com/us/en/support-downloads/rfid/rfid-handhelds/mc3190-z.html
- https://www.zebra.com/us/en/products/rfid/rfid-handhelds/rfd2000.html
- https://www.zebra.com/us/en/support-downloads/mobile-computers/handheld/tc20.html

Industrial fixed position readers from Impinj or Alien also work well with external antennas.

UHF RFID Modules are another potential option for integrating into your kit:
- https://www.sparkfun.com/products/14066

Additionally there are some (currently untested) SDR based UHF RFID reader implementations:
- https://github.com/AdamLaurie/Gen2-UHF-RFID-Reader
- https://shop.m5stack.com/products/uhf-rfid-unit-jrd-4035

# Challenges

## Physical Access Control System (PACS) Box
We didn't just bring a building in a box, we brought the parking lot as well. There will be a range of different credential technlogies (LF, HF, UHF), some you can get your hands on, and some placed out of reach requiring creativity and determination.  You will need to use a variety of tools (including a UHF RFID Reader/Writer) and techniques to interact with our access control system.

Our facility recently upgraded some of our credentials to a special secure bit format:

```
PFFFFFFFFFFFFFFFFIIIICCCCCCCCCCCCCCCCCCCCP
E E E E E E E E E E EO O O O O O O O O O O
```


### Rules
- Sets of cards will be available at the front table and spread out on a few contestant tables.
- You can interact with the badges, you can interact with the readers, but you can't take the badges to the readers.
- Do not reconfigure the readers.
- THIS IS A LEARNING JOURNEY, HAVE FUN!

There are 16 flags of varying difficulty (maybe more depending on how we're feeling): 

## RFHS_RFID_PACS_LF_Clone
### Physical
Create a working clone of Agent Burrows badge.
### Flag
Flag will be revealed upon presentation of the clone to the correct reader.

## RFHS_RFID_PACS_LF_Visual
### Physical
Use your eyes and then create a working clone of Jack's badge.
### Flag
Flag will be revealed upon presentation of the clone to the correct reader.

## RFHS_RFID_PACS_LF_Box
### Physical
Clone the badge secured in the locked box.
### Flag
Flag will be revealed upon presentation of the clone to the correct reader.

## RFHS_RFID_PACS_LF_Brute
### Physical
Find another valid credential in the system.
### Flag
Flag will be revealed upon presentation of the clone to the correct reader.

## RFHS_RFID_PACS_HF_Elite_Clone
### Physical
Create a working clone of Clarice's badge.
### Flag
Flag will be revealed upon presentation of the clone to the correct reader.

## RFHS_RFID_PACS_HF_Elite_Brute
### Physical
Find another valid credential in the system.
### Flag
Flag will be revealed upon presentation of the clone to the correct reader.

## RFHS_RFID_PACS_HF_PIN_X
### Physical
These challenges involve PIN entry, get creative...
### Hint
<details>
  <summary>Click here to see hint...</summary>
The Road to El Dorado is paved with misconfigurations, but the gate is protected with a PIN, demonstrate mastery over the bits and input a valid PIN on readers without a PIN pad.
</details>

### Flag
Flag will be revealed when the valid PIN is entered on the correct reader.

## RFHS_RFID_PACS_HF_MIFARE_Clone
### Physical
Create a working clone of inmate Gumb's badge.
### Flag
Flag will be revealed upon presentation of the clone to the correct reader.

## RFHS_RFID_PACS_HF_MIFARE_Brute
### Physical
Find another valid credential in the system.
### Flag
Flag will be revealed when the next valid credential is found.

## RFHS_RFID_PACS_UHF_Clone
### Physical
Create a clone of Sue's vehicle tag.
### Flag
Flag will be revealed upon presentation of the clone to the vehicle gate reader.

## RFHS_RFID_PACS_UHF_Brute
### Physical
Find another valid credential in the system.
### Flag
Flag will be revealed when the correct value is presented to the vehicle gate reader.

## RFHS_RFID_PACS_HF_Downgrade_X
### Physical
Execute a downgrade attack on a secure credential.
### Flag
Flag will be revealed upon presentation of the clone to the correct reader.

## RFHS_RFID_PACS_HF_Relay
### Physical
Execute a relay attack on Precious.
### Flag
Flag will be revealed when relayed to the correct reader.

## RFHS_RFID_PACS_HF_SE
### Physical
Extract the contents of Paul's badge...
### Flag
Present the contents for verification to recieve the flag.

## ToothBrush Challenge
###Physical
standby for in room instructions
