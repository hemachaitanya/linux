# linux

* ps -ef

* ps aux | awk '/your_command/ {print $2}' (COMMAND LIKE SLEEP )



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

* lsd  (snap install lsd)
  
* dust (snap install dust)
  
* batcat filename (easily identify the files and folders with colours )
  
* tldr awk (full command syntax)

* man fine (full command syntax)

* tail -f (check all logs)

* smartctl +x harddiskpath | less (sudo apt install smartmontools)

* 2 vms or server-client band width findout by using (iperf -s)

*  mtr <hostname> (vpn cannot connected we use ping and trace route combinations for network connections)

*  lsblk - This shows a hierarchical list of block devices and their partitions, including device names, types, sizes, and mount points

*  lsblk -e7 = it disables loop mounts , only shows main partictions

*  ffmpeg , ffplay (play audios and vedios using terminals)

*  sudo adduser <username>

    to change the password forcefull by using

   * passwd --expire <username>

   * su <username> (it shows the current password and new password)
 
   * cat /etc/passwd | grep <perticular user>   (to serarch the home directory path for perticular user)
 
   * d5gg (in vi editor delete )

   


### trouble

* i want to connect one vpn to docker  ,, at that time its shows logs "your credentials is not correct"

* finally i rectified by time zone (date) on server



* cat <file.name>

* sensors-watch

* rm -rf

* sudo passwd (to assign password for the root)

* 
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


### CPU Monitoring:

top: Real-time view of processes with CPU usage stats.

htop: Enhanced, interactive, and colorized version of top.

mpstat: CPU usage statistics, showing breakdown of CPU time.

iostat: CPU and disk I/O statistics.

sar: Historical CPU and resource usage data.

lscpu: Displays detailed CPU architecture information.

### Memory Monitoring:

free: Shows free and used RAM and swap space.

vmstat: Reports processes, memory, paging, and CPU activity.


ps aux --sort=-%mem: Lists processes by memory usage.

smem: Displays memory usage with detailed breakdowns (PSS, RSS, USS

### Combined CPU and Memory:

dstat: Displays CPU, memory, disk, and network usage.

glances: Real-time monitoring of CPU, memory, disk, and more.

atop: Detailed real-time system and resource monitoring.

### System Info:

cat /proc/cpuinfo: Detailed CPU information.

cat /proc/meminfo: Detailed memory information.

uptime: Shows system uptime and average load.

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

### Basic Network Commands:

ifconfig: Displays and configures network interfaces (deprecated, use ip).

ip a: Shows all network interfaces and their IP addresses.

ping: Tests connectivity to a host by sending ICMP echo requests.

traceroute: Traces the route packets take to a network host.

netstat: Displays network connections, routing tables, and interface statistics (deprecated, use ss).

ss: Displays detailed information about sockets and network connections.

hostname: Displays or sets the system’s hostname.

dig: Queries DNS nameservers for DNS records.

nslookup: Queries DNS records for a domain or IP address.

route: Displays or modifies the IP routing table (deprecated, use ip route).

ip route: Shows or configures the routing table.

curl: Transfers data to or from a server using various protocols.

wget: Downloads files from the web via HTTP, HTTPS, or FTP.

scp: Securely copies files between hosts over SSH.

ssh: Securely connects to a remote machine via SSH protocol.

ftp: Transfers files to and from a remote host using the File Transfer Protocol.

sftp: Securely transfers files over SSH.

iptables: Configures packet filtering and firewall rules.

nmap: Scans networks and hosts to discover open ports and services.

whois: Retrieves domain registration and ownership information.

arp: Displays and manipulates the ARP cache.

mtr: Combines ping and traceroute to provide network diagnostics.

ethtool: Displays or modifies Ethernet device settings.

tcpdump: Captures and analyzes network packets.

iwconfig: Configures wireless network interfaces (deprecated, use iw).


iw: Configures wireless devices and shows their status.

### Network Diagnostics:

ping6: Tests connectivity to an IPv6 host.

iperf: Measures network bandwidth and performance.

tcping: Pings a TCP port on a server to check if it’s open.

netcat (or nc): Utility for reading and writing data across network connections.

### User Management Commands:

Create a new user:


sudo adduser username
Add a new user (lower-level):


sudo useradd username
Modify an existing user (add to group):


sudo usermod -aG groupname username
Remove a user account:


sudo deluser username
Delete a user and their home directory:


sudo userdel -r username
Change a user’s password:


sudo passwd username
Change password expiry information:

sudo chage -l username
Group Management Commands:
Create a new group:


sudo addgroup groupname
Add a new group (lower-level):


sudo groupadd groupname
Delete a group:


sudo delgroup groupname
Remove a group:


sudo groupdel groupname
Add user to a group:


sudo gpasswd -a username groupname
Permissions and Ownership Commands:
Change file/directory permissions:


chmod 755 filename
Change file/directory owner:


sudo chown username:groupname filename
Change group ownership:


sudo chgrp groupname filename
Special Permissions:
Setuid:


chmod u+s filename
Setgid:


chmod g+s filename
Sticky Bit:


chmod +t directoryname
User Information Commands:
Display user ID and group ID:


id username
Show user’s groups:


groups username
Display user information:


finger username
Retrieve user entry from NSS:


getent passwd username
Miscellaneous:
Safely edit the /etc/passwd file:


sudo vipw
Safely edit the /etc/group file:


sudo vigr
Execute commands with superuser privileges:


sudo command

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





