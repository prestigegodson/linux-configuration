# Linux Server Configuration:

Installation of a Linux distribution on a virtual machine and prepare it to host your web application(Item Catalog). It includes installing updates, securing it from a number of attack vectors and installing/configuring web and database servers.

* The EC2 URL is : `http://ec2-18-196-33-29.eu-central-1.compute.amazonaws.com/`
* Local IP address: `http://18.196.33.29/`
* SSH port- `2200`
* Passphrase: iamroot

**Resources -** [Add User and give permissions](https://www.digitalocean.com/community/tutorials/how-to-add-and-delete-users-on-an-ubuntu-14-04-vps)

**Resources -** [update and upgrade the packages](https://wiki.ubuntu.com/Security/Upgrades)

#Software installed and configuration changes made

* updated currently installed packages `sudo apt-get update`
*  changed ssh port to 2200 `sudo ufw allow 2200/tcp` `sudo ufw deny 22/tcp`
* created grader user and gave grader sudo permission
* created SSH key pair for grader using ssh-keygen
* configured local timezone to UTC
* Install and configure Apache to serve a Python mod_wsgi application
* Install and configure PostgreSQL
* created a database user called catalog with password 'iamroot' and gave it limited permission
* installed 
* private key name is linuxCourse
