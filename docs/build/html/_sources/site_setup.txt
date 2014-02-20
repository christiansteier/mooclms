Site Setup
==========

This document will show you how to setup a moodle site.

Moodle Installation
-------------------
Moodle is primarily developed in Linus using Apache, PostgreSQL / MySQL / MariaDB and PHP
Basic Requirements
Sever Hardware

Specific hardware requirements for your project will depend on the volume of anticipated concurrent users and should be discussed with your team IT team if you are hosting the server yourself, or company with whom you are hosting. As minimum are:

Disk space: 160MB free (min) plus as much as you need to store your material. 5GB is probably a realistic minimum.

Memory : 256MB (min) , 1GB or more is strongly recommended. Moodle can support 10 to 20 concurrent users for every 1GB of RAM
Server Software

Operating System : A linux based system is recommended for high performance. Example- CentOS, Redhat, Ubuntu, Debian, Mac OS X . Moodle can also be installed on Window 7 / 2012

Web server :  Apache is recommended . Others also wok such as IIS, lighttpd, nginx, cherokee, zeus and LiteSpeed.

PHP : Minimum version is 5.3.3. recommended PHP 5.5 and newer if available.

Database : Minimum versions of following -

    MySQL - version 5.1.33 (mostly recommended)
    PostgreSQL - version 8.3 (mostly recommended)
    MariaDB - version 5.3.5 ( drop-in replacement for Oracle's MySQL)
    MSSQL- version 9.0 (fully supported but documentation and online help are not as comprehensive)
    Oracle - version 10.2 (not recommended)

Browser : Mimimum browser for accessing Moodle: recent firefox, Internet Explorer 9, Safari 6, recent Gooogle Chrome 11 .
Set up your server

Depending on your particular choices of software set up your basic server . If you are using a hosted server all this should be done for you by your hosting provider.
Download and copy files into place

    Download your required version from http://download.moodle.org/ and unzip it .
    Then place the whole folder in your web server documents directory, in which case the site will be located at http://yourwebserver.com/moodle , or you can copy all the contents straight into the main web server documents directory, in which case the site will be simply http://yourwebserver.com .
    Secure the Moodle files: it is vital that the files are not writeable by the web server user. Files are owned by administrator / superuser and are only writeable by them, readable by everyone else. If you want to use built-in ad-on installer you need to make the directory writeable by web server user.

Create an empty database

Create a new, empty database for your installation. You need to find and ake a note of following during information for final installation stage :

    dbhost - the database server hostname. Probably ' localhost ' if the databse and web server are the same machine, otherwise the name of the database server.
    dbname - the database name. Whatever you called it example - moodle .
    dbuser - the username for the database.
    dbpass - the passowrd for the above user

Create the data (moodledata) directory

Moodle requires a directory to store all of its files (all your site's uploaded files, temporary data, cache, session data etc.). The web server needs to be able to write to this directory. So create a directory and set the permissions for anyone on the server to write here. 
Start Moodle Install

    Go to your Moodle's main URL using a web browser.
    The installation process will take you through a number of pages. You should be asked to confirm the copyright, see the database tables being created, supply administrator account details and supply the site details. The database creation can take some time - please be patient. You should eventually end up at the Moodle front page with an invitation to create a new course.


Technical Specification
------------------------


Managing a Moodle Site
-----------------------


Advanced Features
------------------

