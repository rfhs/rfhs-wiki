#Virtual WiFi

Log in to your existing account or create a new one on our scoreboard: https://scoreboard.rfhackers.com/?wtf=login; once you are logged in, click the heading with your user name (https://scoreboard.rfhackers.com/?pita). Follow the directions to provision a new vm (below modifying user settings, above the user scoreboard). Click on the rather small button labeled "provision".
The page will change and indicate "VM Instance provisioning..." and will auto refresh back to the user page.  The SSH keys will be provisioned now and you must download them to your machine.  Follow the directions on the user page just below the SSH Private Key.
The virtual environment takes several minutes to complete, please be patient.  Refresh the page every once in a while to see if it has completed.
Once provisioning is complete, you will see a block of infomation which tells you how to connect to the virtual environment using ssh or your web browser.
There will also be two new buttons below the connection table.  "Reboot" will reboot your virtual environment if something is broken and reset you to a default state (*you will lose your changes and any files*).  "Destroy" will completely erase your virtual environment, this will automatically happen at the end of the game, or you can do it when you are done accessing the game.

=SSH Access=
The game environment can be accessed over ssh or http. If you prefer ssh, here are some helpful tips:

[] The basic access example on the website will get you connected: ssh -i WCTF_Key root@<your_randomly_assigned_hostname>.contestant.rfhackers.com -p 2201
[] Additional ssh flags can be used to enhance the experience.  For example, X11 forwarding can be enabled by adding "-X".  Some users may need to bypass X11 security restrictions and use "-Y" instead, depending on the setup on your machine.  Note: this only works if you are running a local X11 server, typically that means just linux users.  Forwarding X11 means you can run a graphical program in the virtual environment and the display will be pushed back to your local machine through the ssh tunnel for you to interact with.  This can be used, for example, with wireshark.
[] Instead of forwarding all X11 traffic (or in addition), you can forward specific ports from the local host to the remote host.  Adding "-L 2501:localhost:2501" will forward port 2501 on your machine, through the ssh tunnel and connect it to port 2501 on the virtual wifi environment.  This example can be used to connect your local web browser to an instance of kismet running in the virtual wifi environment.  Simply add the -L 2501:localhost:2501 to your ssh invocation and then you can direct your local browser to "localhost:2501" and it will connect through the ssh tunnel to the remote machine's port 2501, where you are presumably running kismet.

=HTTP/VNC Access=
Follow the http access instructions to connect to the virtual environment via http and novnc.  This experience is currently in beta, and may not work as smoothly as desired.  When it does work, it provides a full graphical experience right from your browser.  Please do not trust that this works in any way at all.  Please play with it and report bugs.

Known bugs:
[] Sometimes the screen locks, and refuses to unlock.
[] Lots more bugs, please report them in our discord so we can track and fix them

