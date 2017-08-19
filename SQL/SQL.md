# SQL
MySQL commands and other generic SQL commands

## Table of Contents
* Install MySQL
* MySQL Commands


### Install MySQL
* Download the installation file from [here](https://dev.mysql.com/downloads/mysql/) for Windows
* For CentOS follow the steps [here](https://dev.mysql.com/doc/refman/5.7/en/linux-installation-yum-repo.html)
* For Ubuntu and other linux distribution follow [this](https://dev.mysql.com/doc/refman/5.7/en/linux-installation-apt-repo.html)


### MySQL Commands
* mysql -u root -p : Login into the MySQL server as root user
* mysql -h localhost -P 3306 --protocol=tcp -u root -p : Login into the MySQL server as root as the sppecified host and port
``` bash
mysql -h 10.11.1.90 -P 3306 --protocol=tcp -u root -p
```
* mysqldump -u root -p database-name > database-name.sql : Dump the database into the .SQL file
* mysql -u root -p database-name < database-name.sql : Restore the database with the .SQL file
