# Rtorrent + Rutorrent Auto Install Script by Patrick Kerwood

http://LinuxBloggen.dk/

This is a Bash script i wrote to ease the installtion of rtorrent + rutorrent.

In the installation process you have to choose a system user to run rtorrent.
Also you will get the opportunity of installing 43 plugins/addons. See list further down.
The script add a init script that makes rtorrent start, at a possible reboot, in the 
given username's screen session. Use "service rtorrent-init start" and 
"service rtorrent-init stop" to start and stop rtorrent.

Use rtorrent.auto.install-NEWEST-VERSION for guides or tutorials, as it will allways be the newest version.

**Installation**

Download the script. 

	wget https://raw.github.com/Kerwood/rtorrent.auto.install/master/rtorrent.auto.install-NEWEST-VERSION

Make it executable. 

	chmod +x rtorrent.auto.install-NEWEST-VERSION

Run the script. 

	sudo ./rtorrent.auto.install-NEWEST-VERSION


**Installs**

This scripts installs the following packages with APT.

	openssl 
	subversion
	git
	apache2
	apache2-utils 
	build-essential 
	libsigc++-2.0-dev 
	libcurl4-openssl-dev 
	automake libtool 
	libcppunit-dev 
	libncurses5-dev 
	libapache2-mod-scgi 
	php5 
	php5-curl 
	php5-cli 
	libapache2-mod-php5 
	screen
	unrar-free
	unzip

The script compiles and installs xmlrpc-c from svn.  
Installs rtorrent-0.9.3 and libtorrent-0.13.2, from github.  
Installs rutorrent-3.5 from official site.

**Plugin List**

- 1 - Erase Data Plugin
- 2 - Create Plugin
- 3 - Trafic Plugin	
- 4 - RSS Plugin
- 5 - Edit Plugin
- 6 - Retrackers Plugin
- 7 - Throttle Plugin
- 8 - Cookies Plugin
- 9 - Scheduler Plugin
- 10 - Auto Tools Plugin
- 11 - Data Dir Plugin
- 12 - Track Lables Plugin 
- 13 - Geo IP Plugin
- 14 - Ratio Plugin 
- 15 - Show Peers like wTorrent Plugin
- 16 - Seeding Time Plugin 
- 17 - HTTPRPC Plugin
- 18 - Diskspace Plugin
- 19 - Unpack Plugin
- 20 - Get Dir Plugin
- 21 - Source Plugin
- 22 - Chunks Plugin
- 23 - Data Plugin
- 24 - CPU Load Plugin
- 25 - Extsearch Plugin
- 26 - Theme Plugin
- 27 - Login Mgr Plugin
- 28 - ruTorrent Label Management Suite 
- 29 - NFO Plugin
- 30 - Chat Plugin
- 31 - Logoff Plugin
- 32 - Pause Plugin
- 33 - Instant Search Plugin
- 34 - File Drop (FF > 3.6 & Chrome only).
- 35 - Check Port
- 36 - History
- 37 - iPad
- 38 - Extended Ratio
- 39 - Feeds
- 40 - Media Information
- 41 - RSS URL Rewrite
- 42 - Screenshot
- 43 - RPC
- 44 - Rutracker Check
- 45 - Noty 
- 46 - Task 
- 47 - All Plugins v3.6, Download manually to se which ones. https://bintray.com/novik65/generic/ruTorrent

**Version 2.0.4**  
Fixed the OS check, so now it should be working as intended. 
All plugin dependencies are now installed.

**Version 2.0.2**  
Script is updated so that it only downloads and installs 
rtorrent v. 0.9.3, which is the current version that rutorrent supports.

**Version 2.0.1**  
Added apache2-utils to the package managers install list.

**Version 2.0.0**  
The script now uses an init script to startup rtorrent at boot, instead of the crontab work around.
Use "service rtorrent-init start" and "service rtorrent-init stop" to start and stop rtorrent.


**Version 1.0.6**

- Script now downloads newest version og libtorrent and rtorrent, via github. Current version: rtorrent 0.9.3
- Updated to download Rutorrent 3.6
- Updated all plugins
- Added more plugins

**Version 1.0.5**  
BUGFIX - Directory path for "All plugins" plugin.

**Version 1.0.4**

- 10 new plugins added to list.
- All plugins updatet to newest version.


**Version 1.0.3**

- Added unzip and unrar-free to the installation list.
- Updated "Logoff" plugin to 1.3
- Add right permissions to rutorrent folder.

