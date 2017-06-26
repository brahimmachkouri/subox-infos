![SuBoxes](https://raw.githubusercontent.com/brahimmachkouri/subox-infos/master/images/vagrant-virtualbox-debian.png)

![SuBox](https://raw.githubusercontent.com/brahimmachkouri/subox-infos/master/images/subox3.png)

SuBox is a (BETA) pre-configured Vagrant Box with a full array of features to get you up and running with Vagrant in no time. 

## Get Started

It's easy :

1. Download and Install [Vagrant](https://www.vagrantup.com/downloads.html)
2. Download and Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

Then, in a terminal, just clone the repo and run vagrant up :

```
$ git clone https://github.com/brahimmachkouri/subox my-project
$ cd my-project
$ vagrant up
```

Then visit [http://192.168.33.11](http://192.168.33.11 "SuBox HomePage")

## License 

MIT License

## Features

* Debian 9
* Apache 2.4 (mod_proxy_fcgi activated)
* SSH
* PHP 7.0 (php7.0-fpm), PHP errors On, MSSQL client ready, [PsySH](http://psysh.org/)
* MariaDB 10.1, Sqlite3
* Git, Go lang in the box
* laravel, symfony command line tools included
* PHPMyAdmin, PHPUnit, [composer](https://getcomposer.org/doc/01-basic-usage.md), [wp-cli](https://make.wordpress.org/cli/handbook/quick-start/), [drush](http://www.drush.org/en/master/usage/)
* Email catching with [MailHoge](https://github.com/mailhog/MailHog) : your mails are captured and displayed in a web interface
* [Ansible](https://www.ansible.com) in the box, so you can use [Ansible Galaxy](https://galaxy.ansible.com/list#/roles?page=1&page_size=40&order=-download_count,name) to customize your box
* Virtualbox additions installed
* supervision : [monit](https://mmonit.com/monit)
* admin panels : [webmin](http://www.webmin.com)

## Accounts Stuff

| Username  | Password   |
|-----------|------------|
| vagrant   | vagrant    |
| root      | root       |

## MariaDB Stuff

| PHPMyAdmin URL | http://192.168.33.11/phpmyadmin |
|-----------|------------|
| Hostname  | localhost  |
| Username  | root       |
| Password  | root       |
| Database  | mabase     |

## Development Tools (Beta)

* Yarn, Node.js, nvm, gulp, grunt, bower, webpack, yo... 
> Even though these are packaged into the Vagrant box, we always recommend running node and any packages from your local machine and not within the box. This is strictly a performance thing. They only exist as helpers if you don't/can't set those up.

## Development Stuff

* Just put your files (PHP, HTML, JS...) in the **public** directory (in the box : /var/www/public, or in the **public** directory that you can see next to the Vagrantfile)

![Public directory](https://raw.githubusercontent.com/brahimmachkouri/subox-infos/master/images/public4.png)

* You can enter the box using ssh :
```
vagrant ssh
```
Or :
```
ssh vagrant@192.168.33.11
```

## Frameworks Ready

You have to connect to the box via ssh to use the following tools.

* Laravel : 
```
install_laravel
```

* Symfony : 
```
install_symfony
```

* Code Igniter : 
```
install_codeigniter
```

## CMS Ready

You have to connect to the box via ssh to use the following tools.

* Wordpress via [wp-cli](https://make.wordpress.org/cli/handbook/quick-start/) : 
```
cd /var/www/public
wp core download --locale=fr_FR
```
* October CMS via composer : 
```
cd /var/www
rm -fr public
composer create-project october/october public
```
* Prestashop : 

```
cd /var/www
rm -fr public
git clone https://github.com/PrestaShop/PrestaShop.git public
cd public
composer install
```

## Supervision Stuff

* Monit : http://192.168.33.11:2812

## Admin Panels

* Webmin : https://192.168.33.11:10000

## [MailHog](https://github.com/mailhog/MailHog) Stuff

Just connect to [http://192.168.33.11:8025](http://192.168.33.11:8025)

Inspired by Scotch Box. ;)
