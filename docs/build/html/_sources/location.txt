Location
=========
You are here *Administration > Site administration > Location > Location settings*. 
This menu item allows you to specify the default country location and also time zones.

Location Settings
------------------

  * Default timezone - This sets the default time zone for date display.

  * Force default timezone - Pull down menu to force the user to be in a specific timezone or allow users to individually select their timezone.
 
  * Default country - Select the country to appear by default on a new user account page form.

  IP address lookup 
  
  * GeoIP City data file - Location of GeoIP City binary data file. This is a non-invasive way to determine geographical and other information about Internet visitors in real-time. This file is not part of Moodle distribution and must be obtained separately from MaxMind. There is a GeoIPLite version for free.
  
  * Google Maps API key - Google Maps for IP address lookup visualization key. The Google Maps API lets you embed Google Maps with JavaScript. This is free. 
    
    After updating the information in this section, IP's that are displayed as a link, such as in reports, when clicked will open new window with a Google Map indicating the location of the IP, if found and if not a private address. 


Update Timezone
----------------
The update timezones page *Administration > Site administration > Location > Update timezones* provides administrators with the option to update their local database with new information about world timezones. This is important because of daylight saving changes that many countries use.

If the update is completed with success, Moodle will inform you how many entries were updated and which location was used as a source. 






