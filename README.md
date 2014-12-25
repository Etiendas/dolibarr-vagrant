dolibarr-vagrant
================

Vagrant machine configured for Dolibarr development built with [PuPHPet](http://www.puphppet.com)

### How to use
Mimic the following directory structure

```
|
\-- dolibarr (your copy of dolibarr project)
\-- dolibarr-vagrant (your copy of dolibarr-vagrant project)
```

Now you are ready to start you Vagrant machine.

Remember to update the OS regularly and to add the vhost dev.dolibarr.org to your hosts file. [How?](http://en.wikipedia.org/wiki/Hosts_%28file%29#File_content)

### Stack
* OS: Debian Wheezy 7.5 x64
* HTTP server: Apache 2.4.10
* PHP: 5.5.20-1~dotdeb.1
* DB: MySQL 5.6.21-1~dotdeb.1
* XDebug
* Xhprof
* Mailcatcher 0.5.12
* Composer
* Adminer 4.1.0

### Usage
* IP: 192.168.42.101
* Vhost: dev.dolibarr.org
* Root user: root
* Root password: root
* Configured DB users:
	* user/user for db dolibarr
	* root/root
* Initial dolibarr data: dev/initdata/mysqldump_dolibarr-3.5.0.sql

#### Mailcatcher
Configure Dolibarr to send all emails through SMTP 127.0.0.1 with port 1025 with user admin and no password.
You can access MailCatcher to read all outgoing emails at http://192.168.42.101:1080

#### Adminer
Adminer is a MySQL web client. You can access it through http://192.168.42.101/adminer/

#### XHProf
XHProf is a function-level hierarchical profiler for PHP. You can access it through http://192.168.42.101/xhprof/xhprof_html/