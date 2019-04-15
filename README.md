Townhall: the Stakeholder Democracy
===========================

**ESE Senior Design Team 17**

## Quickstart

townhall is compatible with nearly all GNU/Linux servers with Apache, MySQL, and PHP. Simply clone the repository (with `git clone https://github.com/stakeholderdemocracy/townhall`) in your Apache public HTML directory and then navigate to `/index.php` to auto-configure. 

If extra permissions are needed to create MySQL tables, log in to your SQL console and create them with these commands, changing `<PASSWORD>` to your database password:

```
CREATE DATABASE `townhall`;
GRANT ALL ON `townhall`.* TO `townhall_dbuser`@localhost IDENTIFIED BY '<PASSWORD>';
FLUSH PRIVILEGES;
```

## Alternative option
Townhall is also available as docker image. The platform is built inside an Ubuntu 14.04 docker image with a fully functional LAMP stack. The setup is easy and it involves running the following commands. 
**Note**  
Please make sure that you have docker installed on your machine.  

1. **Pull the docker image**  
```
docker pull slilan96/townhall-lamp-stack
```
2. **Launch the docker image from your terminal **
```
docker run -p <HOST_PORT>:80 -t -i slilan96/townhall-lamp-stack /bin/bash
```

3. **Restart the apache server and mysql**
```
sudo service mysql restart
sudo service apache2 restart
```

**And you are good to go!**



## License

To be as free and transparent as possible for all local governments, the townhall platform is licensed under the GNU General Public License, version 3 only.
