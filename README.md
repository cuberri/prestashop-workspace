Description
===========

This repository contains a [Prestashop](http://prestashop.com/) development workspace.

This is basically a Vagrant box (Ubuntu 12.04 LTS [hashicorp/precise32](https://vagrantcloud.com/hashicorp/precise32)) provisioned by [Ansible](http://www.ansible.com/) with :

* Apache2
* PHP5
* MySQL5
* phpMyAdmin hosted at /phpmyadmin

The hostname set is `prestashopbox` in a `public_network` config.

Requirements
------------

You need python and the amazing [Ansible](http://www.ansible.com/) tool installed on your system for the box to be provisioned. Ansible installation is a matter of seconds with your package manager. `git clone` does the job too :thumbsup: See the [ansible github project page](https://github.com/ansible/ansible/).

Usage
-----

* Clone this repository

```
$ git clone git@github.com:cuberri/prestashop-workspace.git
```

* Boot the vm (Vagrant may ask for the network interface to use, then it's up to you)

```
prestashop-workspace $ vagrant up
```

* Point your browser to `http://prestashopbox/`

* phpMyAdmin is accessible at `http://prestashopbox/phpmyadmin`

Notes
-----

**Please note that this repository is not intended for production. It does not provide any secured environment at all.**

This is a ~~quick~~ as fast as possible start project in order to play with [Prestashop](http://prestashop.com/).

Also, the ansible provioning is very basic and intentionally not "clean", meaning I will not recommend using the playbook as is :P
