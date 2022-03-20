

# General Information

[Radio Frequency Identification](https://en.wikipedia.org/wiki/Radio-frequency_identification) refers to a set of technologies used to wirelessly identify and track tags, and the things that the tags are attached to. Many RFID tags are passive devices, which use electromagnetic induction to wirelessly power the tag from energy provided by the tag reader. There are also active RFID tags, which have their own power source, and typically have longer range than passive tags. RFID tags are used in many different use cases, such as physical access control, [animal identification](https://en.wikipedia.org/wiki/ISO_11784_and_ISO_11785), inventory tracking, public transit passes, [e-passports](https://en.wikipedia.org/wiki/Biometric_passport), vehicle toll passes, and more.

## Frequency Ranges

### LF 120-150 kHz.
Most common LF RFID cards operate at 125kHz. Some common examples include HID Prox, Indala, and HiLetgo EM4100 cards.

### HF 13.56 MHz
There are a number of HF RFID technologies based on the ISO/IEC 14443 standard, which operate at 13.56 MHz. MIFARE Classic, MIFARE Ultralight, and HID iClass are some common technologies that operate in 13.56 MHz. Many public transit cards, other physical access control cards, and NFC also operate in this frequency range.

### UHF 865–868 MHz (Europe) 902–928 MHz (North America)
UHF RFID tags are typically used when longer read distances are required, as compared to LF and HF tags. EPC Gen 2 is one RFID technology that uses this frequency range for passive tags. These tags can be used to track inventory items such as clothing. Tags in this range are also sometimes used in garage access stickers for parking garages. Active RFID tags are also more common in this frequency range, and are frequently used for toll road passes.

## Standards

[ISO/IEC 14443](https://en.wikipedia.org/wiki/ISO/IEC_14443)  
[ISO 11784 and ISO 11785](https://en.wikipedia.org/wiki/ISO_11784_and_ISO_11785)

# Tutorials

[Lab 401 Proxmark Basics Series](https://lab401.com/blogs/academy/tagged/proxmark-basics)

# Tools

[Proxmark3](https://github.com/RfidResearchGroup/proxmark3) - LF and HF RFID swiss-army tool. Read, clone, emulate, sniff, analyze, and more.

[Keysy](https://tinylabs.io/keysy/) - LF RFID Cloner / Emulator

[Chameleon Tiny Pro](https://hackerwarehouse.com/product/chameleon-tiny-pro/) - HF RFID Emulator

[ACS ACR122U](https://www.acs.com.hk/en/products/3/acr122u-usb-nfc-reader/) - USB HF RFID reader/writer

[libnfc](https://github.com/nfc-tools/libnfc)

[mfcuk](https://github.com/nfc-tools/mfcuk)

## Android Apps

[NFC Tools](https://play.google.com/store/apps/details?id=com.wakdev.wdnfc&hl=en_US&gl=US) - Read and write HF RFID tags with your phone.

[RFID Tools](https://play.google.com/store/apps/details?id=com.rfidresearchgroup.rfidtools&hl=en_US&gl=US) - Includes client software for the Proxmark3 and Chameleon Mini
