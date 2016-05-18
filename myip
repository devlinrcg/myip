#!/bin/bash
command_1=wget
command_2=curl
if command -v $command_1 > /dev/null; then
        command_wget=$(wget http://checkip.amazonaws.com -qO -)
       	echo -e "I'm using \e[1;33m$command_1\e[0m and your External IP address is \e[1;33m$command_wget\e[0m"
elif command -v $command_2 > /dev/null; then
        command_curl=$(curl -s http://checkip.amazonaws.com)
        echo -e "I'm using \e[1;33m$command_2\e[0m and your External IP address is \e[1;33m$command_curl\e[0m"
else
	read -p "You don't have either $command_1 nor $command_2; should I install them? [Y/N]" yn
case $yn in
	[Yy]* ) if [ -f /etc/lsb-release ]; then
		sudo apt-get install wget curl
		elif [ -f /etc/debian_version ]; then
		sudo apt-get install wget curl
		elif [ -f /etc/redhat-release ]; then
		sudo yum install wget curl
		elif [[ $(uname -r) == *"amzn"* ]]; then
		sudo yum install wget curl
		fi;
		;;
	[Nn]* ) echo "OK, bye!"; exit;;
	* ) 	echo "--"
		echo -e "Please answer \e[1;31mYes\e[0m or \e[1;31mNo\e[0m. Execute myip again"
	 	exit 0;;
esac
fi
