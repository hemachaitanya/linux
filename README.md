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

* 





