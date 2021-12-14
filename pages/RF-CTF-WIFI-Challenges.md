# RF-CTF-WIFI-challenges


This should be considered a general list with general information for both virtual and online/virtual challenges.

All challenges are subject to change and may be available only if the code or equipment is working.
Please check with staff if you have any questions.

## virtual

Log in to your existing account or create a new one on our scoreboard: https://scoreboard.rfhackers.com/?wtf=login; once you are logged in, click the heading with your user name (https://scoreboard.rfhackers.com/?pita). Follow the directions to provision a new vm (below modifying user settings, above the user scoreboard). Click on the rather small button labeled "provision".


The page will change and indicate "VM Instance provisioning..." and will auto refresh back to the user page.  The SSH keys will be provisioned now and you must download them to your machine.  Follow the directions on the user page just below the SSH Private Key.


The virtual environment takes several minutes to complete, please be patient.  Refresh the page every once in a while to see if it has completed.


Once provisioning is complete, you will see a block of infomation which tells you how to connect to the virtual environment using ssh or your web browser.


There will also be two new buttons below the connection table.

"Reboot" will reboot your virtual environment if something is broken and reset you to a default state (*you will lose your changes and any files*).

"Destroy" will completely erase your virtual environment, this will automatically happen at the end of the game, or you can do it when you are done accessing the game.

## =SSH Access=


The game environment can be accessed over ssh or http. If you prefer ssh, here are some helpful tips:

* The basic access example on the website will get you connected: ssh -i RFCTF_Key root@<your_randomly_assigned_hostname>.contestant.rfhackers.com -p 2201


* Additional ssh flags can be used to enhance the experience.  For example, X11 forwarding can be enabled by adding "-X".  Some users may need to bypass X11 security restrictions and use "-Y" instead, depending on the setup on your machine.  Note: this only works if you are running a local X11 server, typically that means just linux users.  Forwarding X11 means you can run a graphical program in the virtual environment and the display will be pushed back to your local machine through the ssh tunnel for you to interact with.  This can be used, for example, with wireshark.


* Instead of forwarding all X11 traffic (or in addition), you can forward specific ports from the local host to the remote host.  Adding "-L 2501:localhost:2501" will forward port 2501 on your machine, through the ssh tunnel and connect it to port 2501 on the virtual wifi environment.  This example can be used to connect your local web browser to an instance of kismet running in the virtual wifi environment.  Simply add the -L 2501:localhost:2501 to your ssh invocation and then you can direct your local browser to "localhost:2501" and it will connect through the ssh tunnel to the remote machine's port 2501, where you are presumably running kismet.


## =HTTP/VNC Access=


Follow the http access instructions to connect to the virtual environment via http and novnc.  This experience is currently in beta, and may not work as smoothly as desired.  When it does work, it provides a full graphical experience right from your browser.  Please do not trust that this works in any way at all.  Please play with it and report bugs.


### Known bugs:

* Sometimes the screen locks, and refuses to unlock.


* Lots, etc. more bugs, please report them in our discord so we can track and fix them

## ==RF CTF Wifi Challenges==


The entire virtual wifi environment is fair game.


If you can see it, you probably want to hack it.


The challenges are specifically following the ESSID naming convention "RFHS_CTF_##" where ## is a number from 00 through 18 (numbers do NOT indicate difficulty).


Each of these wifi devices will offer a different configuration or challenge.


Please use the included dictionary file for all password cracking needs, you will find it conveniently in your home directory in the virtual environment.


Beginner level challenges for the most common configs are specifically available as "RFHS_CTF_WEP" and "RFHS_CTF_WPA".  These challenges are lower point value but great for starting out or practicing before attacking the main challenges.  The simple step-by-step guides available via google should work well for these, while the main challenges often require some additional finesse.

## Flag


* For WEP based challenges, submit the wep key in ascii or hex.  If you submit in hex, it should be all upper case with no separaters. (FEED00C0FFEE not fe:ed:00:c0:ff:ee)


* For WPA based challenges, submit the wpa passphrase (PSK/SAE) or user password (Enterprise)


* For challenges without a shared key (open, etc), there is a user passing credentials in a cleartext format, sniff it out and submit the password.


* You can connect to RFHS_CTF_12 and navigate to the router from a web browser for a flag.

## Hints


<details>
  <summary>Click here to see hint</summary>


* Always be collecting.  You have multiple wifi cards, USE THEM.


* Ensure the tools you are using are modern.  The protocols we are using are modern, you need modern tools to see things correctly


* Kismet is your friend.  Aircrack-ng is a good acquaintance but not always a friend.


* There are devices for RFHS_CTF_00 through RFHS_CTF_18 *inclusive*, no numbers are missing.  Find it.


* If you get stuck, ask for help in discord.  It's always worth trying.


</details>
