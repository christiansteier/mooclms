.. _mobile_web_services:

Mobile Web Services
====================
Moodle comes with a built-in web service designed for mobile applications. It is required to run the official Mobile app. Enable it only if you want people to use the official app or if a third party app explicitly requires it. 

Enabling mobile web services
------------------------------
A site administrator first must enable mobile web services:

    In *Administration > Site administration > Plugins > Web services > Mobile*
    Check "Enable mobile web services" and then
    Click Save. 
    
What happens when the service is enabled
------------------------------------------
Enabling the mobile web services will automatically:

    * enable the web services system (*Administration > Site administration > Advanced features*)
    * enable the built-in external service called 'Mobile web services' - you should see this new mobile service listed as enabled
    * enable the xml-rpc protocol (for backward compatibility with unmaintained My Moodle app)
    * enable the rest protocol
    * allow the 'webservice/xmlrpc:use' capability for authenticated user role
    * allow the 'webservice/rest:use' capability for authenticated user role 
    
Disabling mobile web services
-------------------------------
When you uncheck 'Enable mobile web services', it will automatically:

    * disable the external service called 'Mobile web services'.
    * if 'Mobile web services' was the only external service enabled:
    
        * disable the web services system
        * disable the xml-rpc protocol
        * disable the rest protocol
        * remove the 'webservice/xmlrpc:use' capability for authenticated user role
        * remove the 'webservice/rest:use' capability for authenticated user role 
        
Read about :ref:`Mobile app <mobile_app>`
