# Linux Server Configuration
A [Udacity Full Stack Nanodegree](https://www.udacity.com/course/full-stack-web-developer-nanodegree--nd004) project.  
Configure and secure Linux Sever and Postgresql database to serve a Python Flask application.

## IP address and SSH port
You can find the application at this IP address is *35.180.129.17*
SSH port used to connect to the server is *2200*.

## Complete URL
http://35.180.129.17.xip.io/

## Software installed
See requirements.txt that it's been generated with `pip freeze > requirements.txt`.

## Configuration changes
* Upgrade software.
* Set timezone to UTC.
* Add user grader to give access to Udacity reviewer with SSH key.
* Give user grader sudo permissions by adding it a configuration file grader /etc/sudoers.d/.
* Set up and enable Uncomplicated Firewall to allow incoming connection:
    * SSH on port 2200 (close default port 22 and use 2200 instead)
    * HTTP on port 80
    * NTP on port 123
* Set up Apache2 to serve a wsgi application in /etc/apache2/sites-enabled/000-default.conf.
* Set up Postgresql. Create database and user with permission on this database.
* Install all dependencies.

## Resources
I found really usefull these Digital Ocean tutorials:  
https://www.digitalocean.com/community/tutorials/how-to-set-up-a-firewall-with-ufw-on-ubuntu-14-04  
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-18-04
