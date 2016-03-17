README
============

End of Life
============
Please notice, that this software is not longer supported and maintained since 10/2014!

Developers
============
Sebastian Kraetzig [info@ts3-tools.info]

What is the TS3 InitD Script?
============
It's a LSBInitScripts shell script. If you are restarting or halting your root/vServer, the script will stop you TeamSpeak server instance. If you start your server, the script will also start your TeamSpeak server instance. You also can use this script with the 'service' command as root user. For example: server ts3server status

Stay tuned!
============
Official Project Homepage: www.ts3-tools.info

facebook Fanpage: https://www.facebook.com/TS3Tools

GitHub: https://github.com/TS3Tools/TS3InitDScript

Requirements
============
- Linux (tested on Debian based system)
- root access on your Linux system
- Installed TeamSpeak server

Supports
============
- Debian Wheezy 7.6
- SQLite and MySQL/MariaDB database (set the second parameter in your ts3server_startscript.sh!)

Features
============
- Stops TeamSpeak server instance, if host system has been shutdown
- Starts TeamSpeak server instance, if host is booting and could detect any network
- 'service' script

The script uses the ts3server_startscript.sh of the set instance.

Installation
============

- Save the ts3server file in /etc/init.d/ directory
- Open the script with `nano /etc/init.d/ts3server` and fill out:  `USER="teamspeak"` You have to enter the username, who ownes the TeamSpeak server instance files and if you need them `TS3PATH=""` and `PARAM=""`.
- Make the script executable with `chmod +x /etc/init.d/ts3server`.
- Update the startup config with update-rc.d ts3server defaults.



Donate
============
TS3InitDScript is free software and is made available free of charge. Your donation, which is purely optional, supports me at improving the software as well as reducing my costs of this project. If you like the software, please consider a donation. Thank you very much!

https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=7ZRXLSC2UBVWE
