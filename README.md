VEMP
====

VEMP is a Vagrant Box preloaded with Ubuntu 12.04, Nginx, MySQL, and PHP. Designed as a quick infill development server, it's created for people who want the power of a Linux development VM on Vagrant without the hassle of Puppet, Chef, or Ansible. 

## Quick Start

* Install [Vagrant](http://vagrantup.com/)
* Add the box: `vagrant box add vemp https://dl.dropbox.com/u/2382631/vemp.box`.
* Go in to your site's root directory and create the VM: `vagrant init vemp`.
* Start things up: `vagrant up`.
* SSH In: `vagrant ssh`.
* Start up Nginx: `sudo service nginx restart`.
* You're good to go! You can access your site with 127.0.0.1:5232

## Defaults
By default, VEMP creates a nginx virtualhost `vagrant` which is set to accept any hostname and serves from the `/vagrant` directory (which is the directory in which your Vagrantfile lives).

## Packages Installed
git
nginx_ensite
python-software-properties
php5-common
php5-mysql
php5-xmlrpc
php5-cgi
php5-curl
php5-gd
php5-cli
php5-fpm
php-apc
php-pear
php5-dev
php5-imap
php5-mcrypt
mysql-server
mysqltuner
nginx

## MySQL Defaults
The default root password is `vagrant`.