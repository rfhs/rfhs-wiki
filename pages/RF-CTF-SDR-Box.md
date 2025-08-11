## SDR Box

![RF CTF SDR Box](https://github.com/rfhs/rfhs-wiki/blob/master/files/images/whatsinthebox/SDR-Box.jpg)

## Inventory
* Intel Nuc
* 3x Nuand bladeRF 2.0 micro xA4
  * 3x Nuand BT-100 Bias-tee Power Amplifier
  * 3x Nuand bladeRF 2.0 micro case

## What Does This Box Do?
The Software Defined Radio (SDR) box transmits the SDR challenges for the RF CTF. The Intel Nuc runs [challengectl](https://github.com/rfhs/challengectl) to transmit the challenges using the 3 bladeRF 2.0 micro SDR devices that are attached to the lid of the case.