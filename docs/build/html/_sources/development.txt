Development
============
Developers of Moodle code have some special tools included in the Moodle package to assist them. Most of the tools should ONLY be used on test sites (not production sites).

Experimental
-------------
Moodle includes a few experimental features which a cautious administrator may consider enabling. 
See :ref:`experimental_settings` for details. 

See :ref:`database_transfer` to know how to migrate moodle site from one database to another.



Debugging
-----------
*Settings > Site administration > Development > Debugging*

At certain times a site administrator will need to see more and/or a more complete error message. The default is to show NONE. These messages can also 1) be very confusing to teachers and students when they suddenly appear and 2) can reveal things about your Moodle and web server that should not be common knowledge. Thus use with care and for short periods of time. See :ref:`debugging`  for details. 


Web Service Test Client
-------------------------
*Settings > Site administration > Development > Web Service Test Client*

Admins can simulate external access to their own Web Services using the URL http://yourmoodlesite.org/webservice/testclient.php.

Warning: The test client is not clever! It lets you choose disabled/unavaibled functions (however it behaves well and produces an error in these case). This is normal because clients are going to be bad sometimes so we needed to simulate a bad client! 



Purge All Caches
------------------
*Settings > Site administration > Development > Purge all caches*

Moodle can cache themes, language strings, filters and other bits of information that have been calculated and stored by the web browser. This link forces all user web browsers to refresh their screens of any information that Moodle has cached. Several modules that use cache have settings which will turn off caching for that module. Eliminating or purging caches slows performance. 



Make Test Course
------------------
*Settings > Site administration > Development > Make test course*

This tool creates standard test courses that include many sections, activities, and files.

This is intended to provide a standardised measure for checking the reliability and performance of various system components (such as backup and restore).



Make JMeter Test Plan
-----------------------
*Settings > Site administration > Development > Make JMeter test plan*

The JMeter test plan generator allows you to run performance tests over a Moodle course, it works along with https://github.com/moodlehq/moodle-performance-comparison

This tool is for developer use only and should not be used on a live site. It is disabled unless you set the debugging option to DEVELOPER. 




PHPUnit Tests
----------------
*Settings > Site administration > Development > PHPUnit test*

The purpose of Unit tests is to evaluate the individual parts of a program (functions, and methods of classes) to make sure that each element individually does the right thing. Unit Tests can be one of the first steps in a quality control process for developing or tweaking Moodle code. The next steps will involve other forms of testing to ensure that these different parts work together properly.




XMLDB Editor
--------------
*Administration > Site administration > Development > XMLDB editor*

The XMLDB editor is a tool for developers to easily edit tables/fields/keys/indexes in install.xml files.


