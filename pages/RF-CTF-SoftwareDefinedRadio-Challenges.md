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
Commonly available ham radio software can be used to decode this.  Examples include: fldigi, qsstv, direwolf, minimodem, wsjtx
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

## BROADCAST_n

### Virtual

This challenge does not have a virtual presence.

### Physical

Look in the US Broadcast FM band for WBFM signal.

### Flag

Boardcast FM can do so much more than just audio. Use some readily available open source tools to pull text from various parts of the signal.

### Hint
<details>
  <summary>Click here to see hint</summary>
What makes the title and artist show up when you're listening to a stereo FM station? What is the protocol behind HD Radio? There might not be any flags in the audio itself.
</details>

## POCSAG

### Virtual

Port Range 6570 has a pager, you know, like in the nineties.

### Flag
Capcode from the repeating transmission
Message from the repeating transmission

### Hint
<details>
  <summary>Click here to see hint</summary>
Check out some tutorials on decoding pagers.
</details>

## LRS_PAGER

### Virtual

Port Range 6566 has a restaurant pager system.

### Flag
submit the full packet (hex string), including the sync word (Excluding preamble)

### Hint
<details>
  <summary>Click here to see hint</summary>
Not all pagers use POCSAG.
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


## ISS

This challenge will require you to send a message to the international space station, be digipeated back to earth, and reported on ARISS.net

An amateur radio license is required!
DMs will come from @APRSISS please follow that account to RX your flag!
Your message to the ISS must include the following string to count DEFCON@twitter_handle@














## ZMQ
server is sdr.rfhackers.com ports 6550-6570
[SDR TOOLS](https://github.com/rfhs/rfctf-sdr-tools)



https://zeromq.org/

ZeroMQ (also known as ØMQ, 0MQ, or zmq) looks like an embeddable networking library but acts like a concurrency framework. It gives you sockets that carry atomic messages across various transports like in-process, inter-process, TCP, and multicast. You can connect sockets N-to-N with patterns like fan-out, pub-sub, task distribution, and request-reply. It's fast enough to be the fabric for clustered products. Its asynchronous I/O model gives you scalable multicore applications, built as asynchronous message-processing tasks. It has a score of language APIs and runs on most operating systems.

**Note:** If you're on a low bandwidth connection, it's recommended to save the IQ stream to a file first, then decode the information from the file.

http://www.sigidwiki.com/wiki/



IN PERSON

The Woody stuff:
First person to solve all three Gets the SWAG Antenna.

**Gotenna:**
This challenge will be based on the original gotennas.
There will be several messages playing. You have three challenges


#1 Gotennas Says: This challnges is an open broadcast. You need to send us in human readable exactly what the payload was. For example if the payload is in hex make it human readable this means real words. 

#2 Go Numbers
This is an encrypted message so you probably cant read the message but tell us what the  phone number or gid is for the sending gotenna.
format no country codes in your flags example 5555555555  or 1234567890 

#3 Go gave me
This will be the phone number or GID of the receiving device. 




