# RF CTF Software Defined Radio Challenges

This should be considered a general list with general information for both virtual and online/virtual challenges.

All challenges are subject to change and may be available only if the code or equipment is working.
Please check with staff if you have any questions.



# Challenges

## HAM_DIGITAL_n

### Virtual

Port Range 6550-6555 is running a digital mode commonly used in ham radio.

### Physical

Look for the signal in the US Amateur Radio bands.

### Flag

Properly decoding this signal will give you a readable ascii string which may be submitted to the scoreboard.

### Hint
<details>
  <summary>Click here to see hint</summary>
Commonly available ham radio software can be used to decode this.  Examples include: fldigi, qsstv, direwolf, minimodem, wsjtx.  For help identifying ham digital modes visit the [sigidwiki amateur radio page.](https://www.sigidwiki.com/wiki/Category)
</details>

## HAM_SSTV_1

### Virtual

Port Range 6560 is running a Slow Scan Television mode commonly used in ham radio.

### Physical

Look for the signal in the US Amateur Radio bands.

### Flag

Properly decoding this signal will give you an image that contains a readable ascii string which may be submitted to the scoreboard.

### Hint
<details>
  <summary>Click here to see hint</summary>
Commonly available ham radio software can be used to decode this.  Examples include: fldigi, qsstv, direwolf, minimodem, wsjtx
</details>

## HAM_MORSE_n

### Virtual

Port Range 6556-6559 is running morse code as commonly used in ham radio.

### Physical

Look for the signal in the US Amateur Radio bands.

### Flag

Properly decoding this signal will give you a readable ascii string which may be submitted to the scoreboard. Must be submitted in ALL CAPS.

Hint
<details>
  <summary>Click here to see hint</summary>
.. ..-. ....... -.-- --- ..- ....... -.-. .- -. ....... .-. . .- -.. ....... - .... .. ... ....... -.-- --- ..- ....... -.. --- -. - ....... -. . . -.. ....... .- ....... .... .. -. -
</details>

## HAM_APRS

### Physical

Send and receive APRS packets in the room.  Make sure to follow the instructions listed in the challenge.

<details>
  <summary>Click here to see hint</summary>
Not all software supports all features of APRS, including compression via MIC-E.
</details>


## SDR_ASK_n

### Virtual

Port Range 6561-6564 is running Amplitude Shift Keying.  Capture this signal and use ASK methods to decode it.

### Physical

Look for the signal in the US Amateur Radio bands.

### Flag

Properly decoding this signal will give you a readable ascii string which may be submitted to the scoreboard.

### Hint
<details>
  <summary>Click here to see hint</summary>
You are doing this manually, software examples include audacity, urh, inspectrum, and baudline.
</details>


## POCSAG

### Virtual

Port 6570 has a pager, you know, like in the nineties.

### Physical

This pager can also be found at 444.5 MHz.

### Flag
Capcode from the repeating transmission
Message from the repeating transmission

### Hint
<details>
  <summary>Click here to see hint</summary>
Check out some tutorials on decoding pagers.  Software example multimon-ng.
</details>

## POCSAG_TX

### Physical

Follow the instructions from the pager at 444.5 MHz.

### Flag
Points will be manually awarded upon completion of this challenge.

## LRS_PAGER

### Virtual

Port 6566 has a restaurant pager system.

### Physical

This system is also running at 467.75 MHz.

### Flag
submit the full packet (hex string), including the sync word (Excluding preamble)

### Hint
<details>
  <summary>Click here to see hint</summary>
Not all pagers use POCSAG.
</details>

## LRS_PAGER_TX

### Physical

These are LRS pagers in the RF Village.

### Flag
Tell one of the RF Village Staff that you want to complete this challenge. Trigger the pager they specify based on their directions.

### Hint
<details>
  <summary>Click here to see hint</summary>
You'll need to identify the system that these pagers came from.
</details>

## 802_15_4_RX

There is a simulated industrial sensor, transmitting continuously.

Flag
Submit the flag transmitted by the sensor, which is an ASCII string, transmitted in between the simulated readings.

Hint
<details>
  <summary>Click here to see hint</summary>
What is IEEE 802.15.4, and what tools can you use to receive it?
</details>

## 802_15_4_TX

There is a simulated industrial sensor, transmitting continuously. Spoof a transmission from the sensor to trigger an alarm on the receiver.

Flag
Submit the flag transmitted by the receiver, which is an ASCII string, transmitted after the alarm is triggered.

Hint
<details>
  <summary>Click here to see hint</summary>
This simulated sensor uses a non-standard protocol within IEEE 802.15.4, and there are protections in place to protect against errors. Craft your attack packet carefully.
</details>

## 6LoWPAN_RX

There are devices communicating periodically over 6LoWPAN.

Flag
Submit the flags transmitted over 6LoWPAN (ASCII strings).

Hint
<details>
  <summary>Click here to see hint</summary>
What is 6LoWPAN? What MAC layer protocol does it use?
</details>

## 6LoWPAN_TX

There are devices communicating periodically over 6LoWPAN.

Flag
Join the 6LoWPAN network, and follow the directions to find this flag (ASCII string).

Hint
<details>
  <summary>Click here to see hint</summary>
You will need bidirectional communication, not just packet injection, to obtain this flag.
</details>


## In person SDR Stuff

There are a few challenges that will be hopping around and changing frequencies.



## ISS

This challenge will require you to send a message to the international space station, be digipeated back to earth, and reported on ARISS.net

An amateur radio license is required!
You must join the RFHS Discord (link on our website rfhackers.com)
Your message to the ISS must include the following string to count DEFCON@discord_username@ (you need the @ signs on either side for submission)
There might be a youtube video on this just saying 



## Tempest

Computer set up with fake monitor

You need to caputure the signal off the cable and reproduce the video signal

once you have an image of the screen there will be text on multiple line going from large to small the smaller the text the more points

submit text displayed to flag submission area


## FPV

See What Ive Got
submit what the camera sees into the flag submission


## WOODY SECTION



### Wifi Hot Spot

Part 1
Within Range of our table is a hotspot present finish the statement Broadcast name "woody says XXXXX"
The XXXXX are the flag to be entered

Part 2
Give us the MAC strait hex no dots as the flag

Part 3 (Tentative)
Crack the handshake submit the password as the flag


### TPMS

Part 1

The flag is the full TPMS hex identifier not including the preamble
put into flag submission in hex

Part 2

The flag is whole number PSI followed by Temperature
put into flag submission
example 100200

Part 3

Flag
Provide the entire hex code from the very first character from preamble through checksum that will give you 4psi to Woody to confirm
put into flag submission in hex

### Ford Key Fob

Key Fob A will provide a lock and unlock signal
Key Fob B will provide a lock signal

Flag
you will need to provide the full character set including the identifier of Keyfob B and the characters that represent the unlock sequence and nothing that follows
put into flag submission in hex

***SEE WOODY***

***FOLLOW ON FOR KEYFOB FOX***

The keyfob identifier from Keyfob B will be the Keyfob you are tracking down.



### Make Ford Key Fob Speak

This is a tough one

Part 1
There is an RFID emitter on the front table

Flag
you must capture the signal and demod it
submit full hex to flag submission

Part 2

not dependent on part 1

Use the RFID signal that you received in part one can be used to complete this challenge with the fob on the table

Flag
submit the first 16 characters of hex of key identifier and the command it gave not counting preamble




### Hit My Caddy

This is a tough one

Keyfob A will broadcast a lock and unlock an another lock

Keyfob B will broadcast a lock

Each identifier is less than 20 bytes


Flag
Keyfob A identifier

Keyfob B identifier

Including preamble provide the unlock sequence for Keyfob B

put into flag submission in hex for each keyfob


### LORA

Flag
Submit the hex message for the LORA no MAC no date time stamp


### IRIDIUM (Maybe if we are lucky)

will announce and update when ready



## ZMQ
server is sdr.rfhackers.com ports 6550-6570
[SDR TOOLS](https://github.com/rfhs/rfctf-sdr-tools)

These ZMQ receivers can be opened in GNUradio and used to modify a signal into a visible and audible format. The virtual machines used for the virtual wifi *can* be used, but performance will be poor.  If possible, it is recommended to use Gnuradio on your local computer for better performance.

By modifying the 'port' variable, you can access each of the different challenges.

https://zeromq.org/

ZeroMQ (also known as ØMQ, 0MQ, or zmq) looks like an embeddable networking library but acts like a concurrency framework. It gives you sockets that carry atomic messages across various transports like in-process, inter-process, TCP, and multicast. You can connect sockets N-to-N with patterns like fan-out, pub-sub, task distribution, and request-reply. It's fast enough to be the fabric for clustered products. Its asynchronous I/O model gives you scalable multicore applications, built as asynchronous message-processing tasks. It has a score of language APIs and runs on most operating systems.

**Note:** If you're on a low bandwidth connection, it's recommended to save the IQ stream to a file first, then decode the information from the file.

http://www.sigidwiki.com/wiki/



IN PERSON
