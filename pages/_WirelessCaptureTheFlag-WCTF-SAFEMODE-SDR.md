# DEFCON28-SAFEMODE-SDR





   ## ZMQ
   server is sdr.rfhackers.com ports 6550-6580
   [SDR TOOLS](https://github.com/rfhs/wctf-sdr-tools/)



   https://zeromq.org/

   ZeroMQ (also known as ØMQ, 0MQ, or zmq) looks like an embeddable networking library but acts like a concurrency framework. It gives you sockets that carry atomic messages across various transports like in-process, inter-process, TCP, and multicast. You can connect sockets N-to-N with patterns like fan-out, pub-sub, task distribution, and request-reply. It's fast enough to be the fabric for clustered products. Its asynchronous I/O model gives you scalable multicore applications, built as asynchronous message-processing tasks. It has a score of language APIs and runs on most operating systems.

   http://www.sigidwiki.com/wiki/


# FLAG SUBMISSION

## LRS

For lrs, submit the full packet, including the sync word
(Excluding preamble)

## POCSAG

For pocsag, submit message as 1 flag, capcode as a 2nd flag

## WOODY BOXES

#### BOX1

Box1 easy removed

Tell me what the ID in HEX is?

Tell me the state?

What is the normal operating freq in Mhz just the Number of the device (non virtualized)?

“SDR_BOX_1_FINAL”
Use the signal from SDR_BOX_1 challenge and DM Woody in discord the command line string that will have your team name as the model name and demodulate to the screen on RTL_433.  In the unlikely event you are correct Woody will send you a flag to input.  This is a manual verification patience is required.



#### BOX2

Flags:

What is the modulations no spaces no hyphens?

Tell me what type of device does this control?

What is the complete hexcode?


#### BOX3

Flags:

What is the modulation?

Is the device currently in RTL_433?

What letter would you use to add the device to your search.








--------------------------------------------------------
## ISS

This challenge will require you to send a message to the international space station, be digipeated back to earth, and reported on ARISS.net

An amateur radio license is required!
DMs will come from @APRSISS please follow that account to RX your flag!
Your message to the ISS must include the following string to count DEFCON@twitter_handle@


## Remote SDR Challenges
   * There are several IQ streams available on ports 6550 though 6565.
   * The IP address of the ZMQ Server is x.x.x.x (or hostname would be better)
   * Use a GNU Radio ZMQ Sub Source to connect to the stream and collect the IQ data.
   * Some streams are using Ham Radio protocols to send text.
   * Other streams are raw ASK signals.
   * Demodulate and decode these streams, submit the correct text messages for points.
   * The sample rate of most streams will be 96k Samples per Second
   * Have you checked out our github?

## HF Ham Radio Challenges
   * This year we’re operating under the callsign W3V
   * We’re transmitting some stuff on HF, what frequency and protocol will vary throughout the day.
   * Don’t have an HF receiver at home? That’s ok, many people make theirs available remotely.
   * The WSPR flag will be our standard format WSPR message.
   * The FT8 flag will be our standard format CQ.
   * There are no points for responding to us, but we would appreciate the QSO.

## Virtual Foxhunt
   * What would a WCTF be without a foxhunt?
   * Go to http://defcon.dfsim.net:8080 to be connected to a network of virtual receivers.
   * Use the virtual receivers to geolocate a series of transmitters.
   * More details available at the website above.
