

# General Information
[Software Defined Radio](https://en.wikipedia.org/wiki/Software-defined_radio) (SDR) is a radio communication system where components that have been traditionally implemented in hardware (e.g. mixers, filters, amplifiers, modulators/demodulators, detectors, etc.) are instead implemented by means of software on a personal computer or embedded system.[1]

[1]Markus Dillinger, Kambiz Madani, Nancy Alonistioti (2003). Software Defined Radio: Architectures, Systems and Functions. Wiley & Sons. p. xxxiii. ISBN 0-470-85164-3.

## General Resources
The [RTL-SDR.com blog](https://www.rtl-sdr.com/) is a great source for news, information, tutorials, and more on all topics related to SDR.

The [GNU Radio Wiki](https://wiki.gnuradio.org/index.php?title=Main_Page) is a wiki focused on all things GNU Radio.

Nuand also has a [BladeRF Wiki](https://github.com/Nuand/bladeRF/wiki) for BladeRF tips and tricks.

The [Ettus Research Knowledge Base](https://kb.ettus.com/Knowledge_Base) for anything USRP or UHD related.

Russ has a number of SDR resources and examples at [sdr.ninja](http://sdr.ninja/)

NotPike has a list of SDR and other RF resources in NotPike's [SDR-Notes](https://github.com/notpike/SDR-Notes)

# Tutorials
[GNURadio Tutorials](https://wiki.gnuradio.org/index.php?title=Tutorials)

[Great Scott Gadgets Software Defined Radio with HackRF](https://greatscottgadgets.com/sdr/)


# Books
[Field Expedient SDR Series](https://www.amazon.com/dp/B078MMXPRY?binding=kindle_edition&ref=dbs_dp_rwt_sb_pc_tukn)


# Hardware
There are many different SDR devices available. The RTL-SDR Blog has a good roundup of general purpose SDR hardware.
[RTL-SDR Blog SDR Roundup](https://www.rtl-sdr.com/roundup-software-defined-radios/)

## RTL-SDR Dongles
[RTL-SDR](https://osmocom.org/projects/rtl-sdr/wiki/Rtl-sdr) generally refers to using USB dongles, based on the Realtek RTL2832U chip, as general purpose SDR receivers. The initial research and development on RTL-SDR was done using inexpensive [DVB-T](https://en.wikipedia.org/wiki/DVB-T) TV tuner dongles. The original TV tuner dongles remain perfectly usable and capable as SDR receivers, however some companies have also made customized dongles with upgrades such as improved oscillators and SMA connectors, intended for use as SDR receivers, for a small increase in price.

[Nooelec NESDR SMArt v4](https://www.nooelec.com/store/sdr/sdr-receivers/nesdr-smart-sdr.html)

[RTL-SDR Blog RTL-SDR Dongles](https://www.rtl-sdr.com/buy-rtl-sdr-dvb-t-dongles/)

[FlightAware Pro Stick Plus](https://flightaware.store/products/pro-stick-plus) is an RTL-SDR dongle with an amplifier and 1090 MHz filter built in. These modifications are intended to improve performance for monitoring [ADS-B](https://en.wikipedia.org/wiki/Automatic_Dependent_Surveillance%E2%80%93Broadcast), but will limit this dongle's performance for other uses.

## TX/RX Capable SDRs
[Great Scott Gadgets HackRF One](https://greatscottgadgets.com/hackrf/one/)

[Nuand BladeRF](https://www.nuand.com/bladerf-2-0-micro/)

[Ettus Research USRP Bus Series](https://www.ettus.com/product-categories/usrp-bus-series/)

The [Portapack for HackRF One](https://store.sharebrained.com/products/portapack-for-hackrf-one-kit) is not a standalone SDR, but it is a useful add-on for the HackRF One that adds a touchscreen display, user controls, a headphone jack, and a micro SD card slot. The [PortaPack Mayhem](https://github.com/eried/portapack-mayhem) firmware is worth looking in to as well.

## RFCat
[RFCat](https://github.com/atlas0fd00m/rfcat) is not quite an SDR, however it is worth mentioning here due to being a very flexible hardware defined radio. Based on the [TI CC1111](https://www.ti.com/product/CC1110-CC1111), RFCat dongles (such as the [YARD Stick One](https://greatscottgadgets.com/yardstickone/)) can transmit and receive signals in a few sub-GHz bands, and with a few specific modulations that are supported by the CC1111.

Frequency ranges (unofficial): 281-361 MHz, 378-481 MHz, and 749-962 MHz bands  
Modulations: ASK, OOK, GFSK, 2-FSK, 4-FSK, MSK  
Data Rate: Up to 500 kbps

[YARD Stick One](https://greatscottgadgets.com/yardstickone/)

There are [other dongles](https://int3.cc/products/rfcat) compatible with RFCat, however the YARD Stick One is the most readily available option at the time of writing.

# Signal Identification and Analysis
[SIGIDWIKI Signal Identification Guide](https://www.sigidwiki.com/wiki/Signal_Identification_Guide)

[Universal Radio Hacker](https://github.com/jopohl/urh) is a tool for capturing, analyzing, demodulating, and decoding unknown wireless signals.

[rtl_433](https://github.com/merbanan/rtl_433), in addition to having built-in decoders for a number of different wireless devices, includes features to save and analyze unknown signals.

# Security Research

Raptor Captor: [Woody - The Ford Hack Raptor Captor video - DEF CON 27 Wireless Village](https://youtu.be/9gfg8gk3lVw), [Hak5: Hacking Ford Key Fobs With a HackRF and Portapack](https://www.rtl-sdr.com/hak5-hacking-ford-key-fobs-with-a-hackrf-and-portapack/)



# Tools

There are many software tools available to work with SDR; too many to put into any single list. The RTL-SDR blog has an extensive list of RTL-SDR supported software in their [The Big List of RTL-SDR Supported Software](https://www.rtl-sdr.com/big-list-rtl-sdr-supported-software/) post. We have also included a few of our favorite SDR tools below.

SDR Basics Breakout
SDR Ninja Software Defined Radio

[gqrx](https://github.com/gqrx-sdr/gqrx) - General purpose SDR receiver with a waterfall display (showing frequency over time), and audio demodulation for AM, FM, and SSB signals, among other things.

[dump1090](https://github.com/flightaware/dump1090) - Receives and decodes ADS-B

[rtlamr](https://github.com/bemasher/rtlamr) - Receives and decodes many common utility meters (electric, gas, water)

[rx_tools](https://github.com/rxseger/rx_tools) - Includes rx_fm, rx_power, and rx_sdr. Based on tools provided by librtlsdr, but with support for more SDR devices.

[TempestSDR](https://github.com/martinmarinov/TempestSDR) - Receive unintentional emissions from computer screens. See also the [RTL-SDR blog post on TempestSDR](https://www.rtl-sdr.com/tempestsdr-a-sdr-tool-for-eavesdropping-on-computer-screens-via-unintentionally-radiated-rf/).

[gr-fosphor](https://osmocom.org/projects/sdr/wiki/fosphor) - Uses OpenCL and OpenGL acceleration, if your system supports it, to provide a Real-Time Spectrum Analyzer (RTSA) like display. This is useful for responsive, wide bandwidth displays. See also the [fosphor - Demo](https://youtu.be/mjD-l3GAghU) video.

[multimon-ng](https://github.com/EliasOenal/multimon-ng) does not interface with SDR hardware directly, but is a useful second step for decoding POCSAG, FLEX, and certain other signals after receiving with something like rx_fm.
