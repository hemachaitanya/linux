# linux


###  TASKS

#### 1. GROUPS IN LINUX

1) PRIMARY GROUP:

 When ever we create some user is called as primary group
2) SECONDARY GROUP :
 When ever we add some user into group is called secodary group

### PACKAGE MANAGER
#### (1) DEB(debian)

apt , dpkg (ubuntu)

* when ever we install packages in /e

* ubuntu source will located in     "/etc/apt/sources.list"

* apt list --installed | grep nginx

* deamon: it's nothing but backend services 

* enable: in case you stop ec2 instance and restart ec2 then status of nginx is also active state

* disable :  in case you stop ec2 instance and restart ec2 then status of nginx is shows inactive (in disable state cannot possible to restart the service)
*  apt remove <package name>
* apt purge < web app>
* apt autoremove < web app>
* sudo kill -9 <process id>
* sudo apt install nginx=1.18.0-6ubuntu14.4
* man apt 
* apt show git (information og git package)
* apt-cache search openjdk
* install specific package for  specific version

        apt-cache madison <web>
        apt install <web | vrsion>
* which apt
* change the password( sudo passwd <user name>)
* 

#### (2)RPM(red hat family)

yum ,rpm (in red hat family)





### (1) task

## named arguments and posissional arguments

*  ping -t google.com (continuously ping)

* process: every process you have unic ips , each process has some cpu and ram

* server: servce is a process but the service have options 
        - when service started eith your s/m  (automatic start)

        - or you manually start the process

        fore ground process:

        background process:
        * when which will start [ex: database and web server runs all the times called deamon and service]

        * enable [service name]
        * start [service name]
        * stop  [services]

## terminal

* power shell(for windows)
* command prompt
* bash (borned again shell  , for linux)
* sh 

## integration testing
## unit test
mvn test (every  java 


developer can test these command)


### /home:
* autherized users  are presented

### /etc
* configure files are present to downloaded applications

### /root
* root users path

### / pdc
* installed any onfiguration files 

### /sbin
* which commands are do by root user
        adduser qtuser
### /var

* find ot the variable or logs files we open /var/logs
   * /var/msgs
### /mnt
* empty file structure you can mount any point
### /media
* mount into default point

###  / boot

* install the software server boot the our files

### /opt

* installed in third party application we using opt 

## linux architechture
* kernal
* shell (it's interface between the you and kernal)
* utilities (applcations)

## commands

* cat <file.name>
* mkdir <folder name>

*  touch {1...n}.txt

*  rm
* - d directory
* - l link
* - normal
* -b lock file 


* if you want to move one dir to another dir you can use <cd>

* ls
* ls -l permssions
* dir inside dir 
        go inside dir and create another dir
        mkdir -p <folder>/<anther-folder>
* cp <source> <destination>

* cat etc/redhat-release - os name

* uname -m (cpu architechture)

* lsblk , df -h (block storage)

* userdel <username>

* groupadd <groupname>

* groupdel <group name>

* find <dir> -type <filename>

*  | grep -r -I in <dir> <text>

* top (load)

* df -kh (k-block size , human readable)

* du -k 

* umask (to set default values ~/.bashrc)

* dig (dns names checking purpose)

*  sudo (lock users)

### 𝐅𝐢𝐥𝐞 𝐒𝐲𝐬𝐭𝐞𝐦 𝐎𝐩𝐞𝐫𝐚𝐭𝐢𝐨𝐧𝐬

ls - List directory contents

cd - Change directory

mkdir - Make directories

rm - Remove files or directories

### 𝐅𝐢𝐥𝐞 𝐏𝐞𝐫𝐦𝐢𝐬𝐬𝐢𝐨𝐧𝐬

chmod - Change file mode bits

chown - Change file owner and group

chgrp - Change group ownership of files

### 𝐏𝐫𝐨𝐜𝐞𝐬𝐬 𝐌𝐚𝐧𝐚𝐠𝐞𝐦𝐞𝐧𝐭

ps aux 

ps -ef

ps - Report a snapshot of current processes

kill - Send a signal to a process

top - Display Linux processes

### 𝐍𝐞𝐭𝐰𝐨𝐫𝐤𝐢𝐧𝐠

ifconfig - Configure network interfaces

ping - Send ICMP ECHO_REQUEST to network hosts

netstat - Display network connections, routing tables, interface statistics

netstat -teln (open ports)

sudo lsof -i:80(specific port running or not)

### 𝐒𝐲𝐬𝐭𝐞𝐦 𝐈𝐧𝐟𝐨𝐫𝐦𝐚𝐭𝐢𝐨𝐧

uname - Display system information

hostname - Display the system's hostname

df - Display disk space usage

### 𝐏𝐚𝐜𝐤𝐚𝐠𝐞 𝐌𝐚𝐧𝐚𝐠𝐞𝐦𝐞𝐧𝐭

apt - Package manager for Debian-based systems (advanced package tool)

yum - Package manager for RPM-based systems(yellowdog updated modifier)

dpkg - Package manager for Debian-based systems(debian package)

rpm - (red hat package manager )

tar - tap archive

cidr   - classless interdomaine 

sha -secure hash algarithem

tcp - transport protocol

### 𝐒𝐡𝐞𝐥𝐥 𝐒𝐜𝐫𝐢𝐩𝐭𝐢𝐧𝐠

bash - GNU Bourne-Again SHell

echo - Display a line of text

grep - Search file(s) for lines that match a given pattern

### 𝐔𝐬𝐞𝐫 𝐚𝐧𝐝 𝐆𝐫𝐨𝐮𝐩 𝐌𝐚𝐧𝐚𝐠𝐞𝐦𝐞𝐧𝐭

useradd - Create a new user or update default new user information

userdel - Delete a user account and related files

passwd - Change user password

### 𝐅𝐢𝐥𝐞 𝐓𝐫𝐚𝐧𝐬𝐟𝐞𝐫

sed -i "old/new/g" >> filename (change file lines)

awk  (i want to print the lines or columns)

awk {print $1}

scp - Securely copy files between hosts

rsync - Remote file synchronization

wget - Retrieve files from the web

### 𝐒𝐲𝐬𝐭𝐞𝐦 𝐒𝐞𝐫𝐯𝐢𝐜𝐞𝐬

systemctl - Control the systemd system and service manager

service - Run a System V init script

chkconfig - Tool for enabling and disabling system services





