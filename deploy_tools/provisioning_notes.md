Provisioning a new site
=========================

## Required packages:

* nginx
* python
* Git
* pip
* virtualenv

eg, on Ubuntu:

    sudo apt-get install nginx git python python-pip
    sudo pip install virtualenv

## Nginx Virtual Host config

* see nginx.template.cong
* replace SITENAME with, eg, staging.my-domain.com

## Upstart Job

* see gunicorn-upstart.template.conf
* replace SITENAME with, eg, staging.my-domain.com

## Folder structure:
Assume we have a user account at /home/username

/home/username
|____sites
    |____SITENAME
        |____database
        |____source
        |____static
        |____virtualenv

