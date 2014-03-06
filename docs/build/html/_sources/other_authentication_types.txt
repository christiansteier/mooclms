.. _other_authentication_types:

Other Authentication Types
===========================

CAS server (SSo)
------------------
Location: *Administration > Site administration > Plugins > Authentication > Manage authentication*

CAS is "Single Sign-on for the Web" and is developed by JA-SIG in an open-source, collaborative manner. CAS is very beneficial in environments where a number of different web applications share a set of common users. If all the web applications were "CASified" a user would log in once and would then be able to move between the various web applications without ever having to present authentication credentials again.


External database authentication
-----------------------------------
Location: *Administration > Site administration > Plugins > Authentication > External database*

This method uses an external database table to check whether a given username and password is valid. If the user does not currently exist in Moodle a new account will be created and their information copied from the external database. 


FirstClass authentication
---------------------------
Location: *Administration > Site administration > Plugins > Authentication > Manage authentication*

FirstClass is a client/server groupware, email, online conferencing, voice/fax services, and bulletin-board system for Windows, Macintosh, and Linux. FirstClass authentication uses the FirstClass Server for the authentication process i.e. to check for user accounts. 


IMAP authentication
---------------------
Location: *Administration > Site administration > Plugins > Authentication > Manage authentication*

IMAP authentication uses a mailing systems IMAP protocol to check for users accounts. This allows direct integrations with technologies such as Microsoft Exchange servers. 


LDAP authentication
---------------------
Location: *Administration > Site administration > Plugins > Authentication > Manage authentication*

This document describes how to set up Lightweight Directory Access Protocol (LDAP) authentication in Moodle. We cover the basic, advanced and some trouble shooting sections to assist the user in the installation and administrating LDAP in Moodle. 


NNTP authentication
---------------------
Location: *Administration > Site administration > Plugins > Authentication > Manage authentication*

NNTP authentication uses the Usenet NNTP protocol to check for users accounts. This allows direct integration with technologies such as Microsoft Exchange, INN, DNews, Diablo, etc. 


PAM (Pluggable Authentication Modules)
----------------------------------------
Location: *Administration > Site administration > Plugins > Authentication > Manage authentication*

With PAM you can use the same user database for different applications log ins (SSO - Single Sign On). PAM also supports different authentication processes as required.

This method uses PAM to access the native usernames on this server. You have to install PAM Authentication Module in order to use this module. 


POP3 server authentication
----------------------------
Location: *Administration > Site administration > Plugins > Authentication > Manage authentication*

POP3 server authentication is a user authentication process i.e. enabling people to login to your Moodle site. This method uses the POP3 mail server for the authentication process ie. check for users accounts. 


RADIUS authentication
-----------------------
Location: *Administration > Site administration > Plugins > Authentication > Manage authentication*

If you get an error message saying: "Warning: The Auth_RADIUS module does not seem to be present", you need to follow these steps:

Using debian-based linux (such as Ubuntu):

  1. Install the following modules: php5-dev php5-auth-pam php5-radius php-pear

        sudo apt-get install php5-dev php5-auth-pam php5-radius php-pear

  2. Install Auth_RADIUS module for pear

        sudo pear install radius Auth_RADIUS

  3. Add the following line to your php.ini file

        extension=radius.so

  4. Restart apache services

        sudo /etc/init.d/apache2 restart
        
        
Shibboleth
------------
Location: *Administration > Site administration > Plugins > Authentication > Manage authentication*

Shibboleth is an Internet2 Middleware Initiative project that has created an architecture and open-source implementation for federated identity-based authentication and authorization infrastructure based on SAML. Federated identity allows for information about users in one security domain to be provided to other organizations in a common federation. This allows for cross-domain single sign-on and removes the need for content providers to maintain usernames and passwords. Identity providers (IdP's) supply user information, while service providers (SP's) consume this information and gate access to secure content. 














