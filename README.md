#conServers.sh#

##Intro##

This is script list all server from html page with table (<td>) and automatc coonect  in selected server.

##Requirements##

1. Linux or MacOSX
2. SSH RSA Key to connect on Server
3. HTML Page with table (Company | Hostname or ip Address| user| port | alias )
	
##How to Install##
	cd ~/
	wget https://github.com/brfso/conServers/archive/master.zip
	unzip conServers-master.zip
	sudo ln -s $PWD/conServers-master/conservers.sh /usr/bin/
	
##How to Use##

	1. Set SSH Key in SSH_KEY in coserver.sh
	2. Change Page to connect (url) in getServers.rb
	3. Execute conServers.sh
		conservers.sh
####To Update Server List	
	To update server list from html page, execute with option -a:
	conserver.sh -a

##toDO##
1. Support connections to windows server (rdesktop, etc)
2. Support to automatic HTML Page update from servers
3. Add Auth HTTP as Option
4. Change parameters to config file
5. Add Automatic detect changes in HTML PAGE and update CSV file