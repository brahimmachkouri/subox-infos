
![SuBox](https://raw.githubusercontent.com/brahimmachkouri/subox-infos/master/images/subox.png)

SuBox is a (BETA) pre-configured Vagrant Box with a full array of features to get you up and running with Vagrant in no time. 

## Quick tutorial

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
* PHP 7.0 (php7.0-fpm), PHP errors On, MSSQL client support
* MariaDB 10.1, Sqlite3
* Git, Go lang in the box
* PHPMyAdmin, PHPUnit, composer, wp-cli
* Beta : Yarn, Node.js, nvm, gulp, grunt, bower, webpack, yo 
* Email catching with [MailHoge](https://github.com/mailhog/MailHog)
* Ansible in the box, so you can use [Ansible Galaxy](https://galaxy.ansible.com/list#/roles?page=1&page_size=40&order=-download_count,name) to customize your box

## Frameworks Ready

* Laravel, Symfony, Code Igniter...

## CMS Ready

* Wordpress, Drupal, October CMS, Magento, Prestashop

## Development Stuff

Just put your files (PHP, HTML, JS...) in the **public** directory 

## MariaDB Stuff

|           |            |
|-----------|------------|
| Hostname  | localhost  |
| Username  | root       |
| Password  | root       |
| Database  | mabase     |

## Accounts Stuff

| Username  | Password   |
|-----------|------------|
| vagrant   | vagrant    |
| root      | root       |

## [MailHog](https://github.com/mailhog/MailHog) Stuff

Just connect to [http://192.168.33.11:8025](http://192.168.33.11:8025)

Inspired by Scotch Box. ;)
