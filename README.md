# Script/Beautifier to get external IP address from command line on Linux
### Prerequisites
**wget** or **curl**
### How it Works
**myip** is a simple script, written in Bash, so you can check your External IP the easy way.  
It checks if you have either **wget** or **curl**, and execute the command against http://checkip.amazonaws.com (which is VERY reliable); if you don't have these commands installed, it will ask you to permit the installation. Upon YES, it consults whether you are using Ubuntu, Debian, CentOS, RHEL or Amazon Linux and install both of them.  
After that, you can run the command again.  
It is **SIMPLE** and, if you don't like it, just execute the commands by yourself and you'll be fine :)  

  If you have any needs or issue to report, feel free!
### Basic installation
```
Just download or git clone the repository, and put myip in your path
```
