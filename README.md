# Aureola

Version : v1.1.3
Date : 11/07/2016

A collection of conky's I made myself and conky's I like that were shared with the community.

These conky's configuration files follow the LUA syntax as mentioned on the conky website for version 1.10 and later versions.

Conky's will be first tested and made on Linux Mint and then tested on other Os's.


# Installation of conky aureola

To get al these conky's to your computer, run the script

	- get-aureola-from-github-to-local-drive.sh


This script will take care of :

	- file management

	- making sure that conky start next time you boot

	- making sure there is a .config/conky folder present

	- making a hidden folder ~/.aureola where all the github files will reside

	- copy/pasting the github files in the hidden folder ~/.aureola




The conky files 'HOME' folder is ./config/conky.

Anything in there will be started by conky.



# Installation of the program conky


If you see nothing then you may still need to install conky.

	sudo apt-get install conky conky-all

	or

run the script provided (which gets more programs to know your motherboard name, etc...)


	- install-conky-and-extra-software.sh


I recommend you use also the conkymanager but there is a but. Read on.

	sudo apt-get install conky-manager

But conky is changing its configuration file to lua syntax. That gives issues at this moment of writing (June 2016).




# Switching the conky

Every conky has an installation script.

The script asks you  if it is ok to delete everything inside folder ~/.config/conky.

Respond with yes. The original files are in ~/.aureola anyway and on github.

Two things will happen after conky has stopped.

	1. current info in ./config/conky will be deleted
	2. new conky files will be copied from  ~/.aureola/...  to ./config/conky 

Conky will restart with new conky configuration file.

If there are dependancies (read software) that is required for the conky to function fully,
it will be installed as well.


# OVERVIEW OF THE CURRENT COLLECTION

The most recent conky come first



# Aureola - Acros

script to get the latest image for spotify and a logo for the distro


![Screenshots](http://i.imgur.com/pyZEPdf.png)



# Aureola - Salis

Working with a lua ring script

![Screenshots](http://i.imgur.com/VPBJ6uV.png)


# Aureola - Lazuli

After the creation of a new icon set i.e Sardi Mono Grey I adapted the colors to go with the icon design.
Sardi icons to be found at https://sourceforge.net/projects/sardi


![Screenshots](http://i.imgur.com/o2Dp2bH.png)



![Screenshots](http://i.imgur.com/2JLL5kl.png)






# Aureola - Sparki

![Screenshots](http://i.imgur.com/GU4ck3k.png)

Credits Willem O








# Aureola - Alva

At the moment of creating this collection I found out that conky had decided to follow the LUA syntax for their configuration files.

Adapted this conky so it is now compliant to the lua syntax. This has a LUA script that draws the rings etc.



![Screenshots](http://i.imgur.com/57QwNug.png)

This is the original conky from EtlesTeam still available in the folder lua.

This is the changed version that will activated standard for ethernet connection.

![Screenshots](http://i.imgur.com/77wMpId.png)


The original conky had wireless link quality and downspeed as bottom gauge.

Since I am working on a pc, I wanted my ethernet connection to show up.

If you want the original laptop conky back with wireless information then rename the rings_text-bg.lua to rings_text-bg-ethernet.lua. And change rings_text-bg-for-wireless.lua to rings_text-bg.lua. Check the name in the lua file for the name of your wireless card. Now it is named <b>wlx0015af414869</b>.

The ethernet conky (the one standard activated) uses <b>enp2s0</b> as ethernet name. It can me also eth0 or eth1 or something else. 

Find out with following command in a terminal

	ip link


In the lua conky I did a netspeed test and adapted my conky max for upspeed and downspeed accordingly.

downspeed 	= 191,19 Mbps  	- in conky 	-	190.000

Upspeed  	=  23,98 Mbps	- in conky 	-	22.000

<a href="http://www.speedtest.net/my-result/5467198314"><img src="http://www.speedtest.net/result/5467198314.png" /></a>






# Home of Conky

https://github.com/brndnmtthws/conky

Configuration Settings

https://github.com/brndnmtthws/conky/wiki/Configuration-Settings

Conky Variables (more as backup)

http://conky.sourceforge.net/variables.html




# Interesting links

http://u-scripts.blogspot.be/

http://crunchbang.org/forums/viewtopic.php?id=16909&p=1

http://crunchbang.org/forums/viewtopic.php?id=39997

http://thepeachyblog.blogspot.be/p/index-or-home-page.html