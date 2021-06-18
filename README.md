# Script/Beautifier to get external IP address from command line on Linux

### Prerequisites

**wget** or **curl**

### How it Works

**myip.sh** is a simple bash script so you can check your External IP the easy way.  
It checks if you have either **wget** or **curl**, and execute the command against https://checkip.amazonaws.com (which is reliable); if you don't have these commands installed, it will ask you to permit the installation. Upon YES, it consults whether you are using Ubuntu, Debian, CentOS, RHEL or Amazon Linux and install both of them.  
After that, you can run the command again.  
It is **SIMPLE** and, if you don't like it, just execute the commands by yourself and you'll be fine :)  

If you have any needs or issue to report, feel free!

### Basic installation

```text
Just download or git clone the repository
$ chmod +x myip
Put myip in one of your directories inside your $PATH;
```

### TODO
