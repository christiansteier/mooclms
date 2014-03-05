.. _using_web_services:

Web services
=============
Web services enable other systems to login to Moodle and perform operations. 

Enabling web services
-----------------------
    1. Access *Administration > Site administration > Advanced features*
    2. Check 'Enable web services' then click 'Save Changes' 

**Note:** For security reasons, web services should only be enabled if you intend to make use of it. 

Enabling protocols
--------------------
Usually external applications that users wish to use dictate which protocols should be enabled.

    1. Access *Administration > Site administration > Plugins > Web services > Manage protocols*
    2. Enable the protocols (SOAP, REST, XMLRPC, AMF, ...) as required 


Enabling web service function documentation
---------------------------------------------
Enabling web service function documentation (also on the Manage protocols page) results in user-specific web service documentation being available for each user on their Security keys page. This option is mainly useful to web service client developers. If nobody is creating a web service client, there is no need to enable this feature.
