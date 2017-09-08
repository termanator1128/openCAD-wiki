This section of the installation guide will cover preparing your environment for a successful openCAD installation.

__Before beginning please update AND upgrade your packages__
`sudo apt update -y && sudo apt upgrade -y`

# Preparing the Environment

1. Install chosen operating system. openCAD can be setup on any Linux based system.

__The openCAD dev team recommends Ubuntu 16.04 LTS__

2. Install `python-software-properties`.

`sudo apt install python-software-properties`

3. Add the nginx PPA repository.

`sudo add-apt-repository ppa:nginx/$nginx`

4. Install packages for a LEMP (nginx, MySQL/MariaDB, PHP) environment.

`sudo apt install git-core nginx mariadb* php-fpm php-mysql phpmyadmin`

If you have gone through the steps and can answer "Yes" to the following statements then you have successfully prepared your environment for openCAD:

1. I can access the default nginx test page.

Go To: [Configure Web Server - nginx](Configure_Web_Server_-_nginx.md)
Go To: [Configure Web Server - Apache](Configure_Web_Server_-_Apache)

# Troubleshooting

**Problem 1:** Unable to access nginx test page or phpmyadmin from the browser.

*Solution:* Check your firewall settings. You may need to allow port 80 through the firewall. To do simply run the following command.

`sudo ufw allow 80; sudo ufw allow 443`
