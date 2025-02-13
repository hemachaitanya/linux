### linux

### all linux commands 
```
    7  alias kgn='kubectl get nodes -o=wide --show-labels'
    8  docker container run -d -P jenkins/jenkins
    9  docker container ls --quiet |awk '{print $1}'
   10  bg %1
   11  touch hema{1..5}.txt
   12  ls -al
   13  echo "hai hema 2" >> hema2.txt 
   14  caat hema2.txt 
   15  cat hema2.txt 
   16  sudo addgroup chaitanya
   17  sudo adduser hema
   18  cat /etc/passwd
   19  cat /etc/group
   20  chgrp chaitanya hema5.txt
   21  chmod 241 hema2.txt 
   22  chmod u+x hema2.txt 
   23  touch script.sh
   24  echo 'sudo apt update && sudo apt install openjdk-17-jdk -y'
   25  echo 'sudo apt update && sudo apt install openjdk-17-jdk -y' >>script.sh 
   26  sudo chmod +x script.sh 
   27  ./script.sh 
   28  mkdir 2017
   29  chown hema:cahitanya hema1.txt 
   30  sudo chown hema:chaitanya hema1.txt 
   31  sudo chown -R hema:chaitanya 2017/
   32  sudo cp hema2.txt hema1.txt 
   33  echo "hlo" >>hema2.txt 
   34  echo "chaitu" >> hema2.txt 
   35  cat hema2.txt 
   36  cut -f1-3 hema2.txt 
   37  cut -f1-1 hema2.txt 
   38  touch file.csv
   39  vi file.csv 
   40  cut -f1-1 file.csv
   41  date
   42  date +"%Y-%m-%d %H:%M:%S"
   43  df-h
   44  df -h
   45  df -i
   46  dd if=/dev/sda of=/dev/sdb bs=64k conv=noerror,sync
   47  dig google.com
   48  dmesg
   49  dmesg | grep usb
   50  du -ah
   51  du -sh
   52  du -ah 2017/
   53  $HOME
   54  HOME=root
   55  $HOME
   56  snap install root-framework
```


### manage access to root user


* sudo login , sudo -i

* sudo useradd username

* id username

* su -,su --login

* lxd init

* lxc import ldap-server.tar.xz

* lxc start ldap-server

* lxc list

* sudo apt update & sudo apt install libnss-ldapd -y

* cat /etc/nsswitch.conf

* cat /etc/nslcd.conf

* id useename

* getent passwd

* getent passwd --service ldap

* getent group --service ldap

* ls /home

* sudo pam-auth-update

* sudo login username

* ls /home

## configure ip address and hostname resolution

* cidr calculator

* ip link

* ip adress

* ip addr

* ip a

* ip -c addr

* ip addr -c

* sudo ip link set dev enp0s8 up

* sudo ip link set dev enp0s8 down

* sudo ip addr add 10.0.0.40/24 dev enp0s8

* sudo ip addr delete fe80::5054::ff::8050/64 dev enp0s8

* sudo netplan get

* ls /etc/netplan

* cat /etc/netplan/50-cloud-init.yaml

* sudo ufw allow 22

* sudo ufw delete 22

* sudo ufw status 

* sudo ufw delete qllow 22

* sudo ufw allow from 10.0.0.0/24 to any port 22

* sudo ufw allow from 10.0.0.0/24

* sudo ufw deny 10.0.0.0/24

* sudo ufw delete 1

* sudo  ufw status numbered

* ip link

* 


,,,
* network:
    ethernets:
      enp0s8:
        dhcp4 false
        dhcp6 false
        addresses:
          - 10.0.0.9/24
       nameservers:
        addresses:
          - to 192.168.0.0/24
            via 10.0.0.100
          - to default
            via 10.0.0.1
  version: 2
  ,,,

* sudo neatplan apply

* sudo netplan try

* sudo netpaln try --timeout 30

* sudo chmod 600 /etc/ne tplan/99-mysettings.yaml

* sudo netplan get

* ip route

* resolvectl status

* sudo vim /etc/resolve.conf      add dns=1.1.1.1.9.9.9.9

* resolvectl dns

* sudo vim /etc/hosts

* ls /usr/share/doc/netplan/examples/static.yaml

* 

## general commands

*  cp source-file-path destination-file-path

*  Copy-Item source-file-path destination-file-path

*  mkdir nameof-directory

*  New-Item name-of-file

*  cat file-name

*  Start-Process ".\ADHAR (1).pdf" (for images)

*  ls | grep "word-of file*"

*  Get-ChildItem | Where-Object { $_.Name -like "*what you want to search*" }

*   rm -rf file-name

*   Remove-Item file-name
  
### codes

Here are signal codes specifications from 

### 1xx to 5xx:

### 1xx - Informational Responses*

- 100 Continue (request received, continue processing)

- 101 Switching Protocols (switching to new protocol)

- 102 Processing (processing request, no response yet)

 ### *2xx - Success*

- 200 OK (request successful)

- 201 Created (resource created)

- 202 Accepted (request accepted,
 processing)

- 203 Non-Authoritative Information (meta-information changed)

- 204 No Content (no content returned)

- 205 Reset Content (reset form)

- 206 Partial Content (partial content returned)

### 3xx - Redirection*

- 300 Multiple Choices (multiple options)

- 301 Moved Permanently (resource moved)

- 302 Found (resource temporarily moved)

- 303 See Other (redirect to different URL)

- 304 Not Modified (resource unchanged)

- 305 Use Proxy (use proxy to access resource)

- 307 Temporary Redirect (temporary redirect)

- 308 Permanent Redirect (permanent redirect)

### 4xx - Client Errors*

- 400 Bad Request (invalid request)

- 401 Unauthorized (authentication required)

- 402 Payment Required (payment required)

- 403 Forbidden (access denied)

- 404 Not Found (resource not found)

- 405 Method Not Allowed (method not supported)

- 406 Not Acceptable (content not acceptable)
- 407 Proxy Authentication Required (proxy authentication)

- 408 Request Timeout (request timed out)

- 409 Conflict (resource conflict)

- 410 Gone (resource permanently removed)

- 411 Length Required (content length required)

- 412 Precondition Failed (precondition failed)

- 413 Payload Too Large (payload too large)

- 414 URI Too Long (URI too long)

- 415 Unsupported Media Type (media type unsupported)
- 416 Range Not Satisfiable (range not satisfiable)

- 417 Expectation Failed (expectation failed)

- 418 I'm a teapot (April Fool's joke)
- 421 Misdirected Request (misdirected request)
- 422 Unprocessable Entity (unprocessable entity)
- 423 Locked (resource locked)

- 424 Failed Dependency (failed dependency)
- 425 Too Early (too early)

- 426 Upgrade Required (upgrade required)

- 428 Precondition Required (precondition required)

- 429 Too Many Requests (too many requests)

- 431 Request Header Fields Too Large (header fields too large)

- 451 Unavailable For Legal Reasons (unavailable for legal reasons)

### 5xx - Server Errors*

- 500 Internal Server Error (server error)

- 501 Not Implemented (method not implemented)

- 502 Bad Gateway (bad gateway)

- 503 Service Unavailable (service unavailable)

- 504 Gateway Timeout (gateway timeout)

- 505 HTTP Version Not Supported (HTTP version unsupported)

- 506 Variant Also Negotiates (variant also negotiates)

- 507 Insufficient Storage (insufficient storage)

- 508 Loop Detected (loop detected)
- 509 Bandwidth Limit Exceeded (bandwidth limit exceeded)
- 510 Not Extended (not extended)

- 511 Network Authentication Required (network authentication)

These signal codes are based on HTTP/1.1 specifications (RFC 7231).

Would you like me to explain any specific code?

# Here are some complete commands to troubleshoot latency and accessibility issues:

 ## Latency Issues*

1. Check system load:

    - `top`
    - `htop`
    - `mpstat -A`

2. Monitor CPU usage:

    - `top -c`
    - `htop -c`
    - `sar -u`

3. Analyze memory usage:

    - `free -m`
    - `vmstat -s`
    - `pmap -d`

4. Inspect disk I/O:

    - `iostat -x`
    - `iotop`
    - `sar -d`
     duet
      -du -hf`

5. Verify network connectivity:

    - `ping -c 10 (link unavailable)`
    - `traceroute (link unavailable)`
    - `mtr (link unavailable)`

6. Check application logs:

    - `tail -f /var/log/app.log`
    - `grep "error" /var/log/app.log`

7. Use profiling tools:

    - `gprof`
    - `Valgrind --tool=memcheck`

*Accessibility Issues*

1. Check firewall rules:

    - `iptables -n -L`
    - `ufw status`

2. Verify port availability:

    - `netstat -tlnp | grep 80`
    - `ss -tlnp | grep 80`

3. Test network connectivity:

    - `telnet (link unavailable) 80`
    - `nc (link unavailable) 80

4. Inspect DNS resolution:

    - `dig (link unavailable)`
    - `host (link unavailable)`

5. Check application configuration:

    - `cat /etc/app/config`
    - `grep "listen" /etc/app/config`

6. Monitor system logs:

    - `tail -f /var/log/syslog`
    - `grep "error" /var/log/syslog`

7. Analyze access control lists (ACLs):

    - `getfacl /path/to/file`

*Networking Commands*

1. `ping -c 10 (link unavailable)` (test network connectivity)

2. `traceroute (link unavailable)` (analyze network route)

3. `netstat -tlnp` (display network connections)

4. `ss -tlnp` (display socket statistics)

5. `tcpdump -i eth0 -n -vv -s 0 -c 100` (capture network traffic)

6. `nc (link unavailable) 80` (test network connectivity)

7. `dig (link unavailable)` (inspect DNS resolution)

*System Commands*

1. `top` (display system load)

2. `htop` (interactive system monitor)

3. `mpstat -A` (display CPU statistics)

4. `vmstat -s` (display memo ry
 statistics)

5. `iostat -x` (display disk I/O statistics)

6. `sar -u` (display system activity report)

7. `sysctl -p` (configure system parameters)

*Application-Specific Commands*

1. `ps aux | grep app` (display process information)

2. `pmap -d` (display process memory map)

3. `strace -c` (analyze system calls)

4. `lsof -i :80` (list open files)

5. `curl -v (link unavailable)` (test HTTP connectivity)

*Troubleshooting Steps*

1. Identify symptoms
2. Gather information
3. Analyze logs
4. Inspect system configuration
5. Test network connectivity
6. Verify application configuration
7. Profile application performance

*Additional Tools*

1. New Relic (application performance monitoring)

2. Datadog (system monitoring)

3. Prometheus (monitoring system)

4. Grafana (visualization platform)

5. Wireshark (network protocol analyzer)

To resolve issues:

1. Identify the root causes

2. Apply fixes or configuration change S

3. Verify resolutions

4. Monitor system performances

5. Document changes

Would you like more information on using these commands or troubleshooting specific issues?

## Here is a sample script that appends a line to delete_user.yml:

<<<<<<< HEAD
Bash Script to Append a Line
```yaml
#!/bin/bash
=======
* ps -ef

* ps aux | awk '/your_command/ {print $2}' (COMMAND LIKE SLEEP )


>>>>>>> 1b5446c911b4ded0aa7c25fa89a4e213bc9fd4eb

# File to modify
PLAYBOOK="delete_user.yml"

# Line to append (this is an example, you can modify it as per your needs)
LINE_TO_APPEND='    - name: Notify user deleted'

# Check if the line is already in the file to avoid duplication
if ! grep -Fxq "$LINE_TO_APPEND" "$PLAYBOOK"; then
  # Append the line to the end of the file
  echo "$LINE_TO_APPEND" >> "$PLAYBOOK"
  echo "Line appended to $PLAYBOOK"
else
  echo "Line already exists in $PLAYBOOK"
fi
```
#### How It Works:

* PLAYBOOK="delete_user.yml": 

Specifies the playbook file you want to append the line to.

* LINE_TO_APPEND='- name: 

Notify user deleted': This is the line that will be appended to the playbook. You can modify this to any content.

* grep -Fxq:

 This checks if the line already exists in the file to avoid appending it multiple times.

* echo "$LINE_TO_APPEND" >> "$PLAYBOOK": 

<<<<<<< HEAD
This appends the line to the playbook if it does not exist.
=======
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
>>>>>>> 1b5446c911b4ded0aa7c25fa89a4e213bc9fd4eb

* How to Run the Script:

Save the above script in a file, for example, append_line.sh.
Make it executable:

chmod +x append_line.sh

* Run the script:

./append_line.sh
This will append the specified line to the delete_user.yml file if it doesn’t already exist.
