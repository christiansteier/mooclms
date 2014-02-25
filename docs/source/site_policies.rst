.. _site_policies:

Site Policies
==============
 
**Protect usernames**
If enabled, when a user attempts to reset their password and enters a username or email address, the following message is displayed: "If you supplied a correct username or email address then an email should have been sent to you." This is to prevent a malicious party from using the interface to determine which usernames and email addresses are in use in valid accounts.

If the protect usernames setting is disabled, when a user attempts to reset their password they are provided with feedback regarding whether an account exists with the username or email address supplied. For example, the message "The email address was not found in the database" may be displayed.

**Force users to login**
If you turn this setting on, all users must login before they even see the Front Page of the site.

**Force users to login for profiles**
Leave this set to Yes to keep anonymous visitors away from user profiles.

**Force users to login to view user pictures**
If enabled, users must login in order to view user profile pictures and the default user picture will be used in all notification emails.

**Open to Google**
Enabling this setting allows Google's search spiders guest access to your site. Any part of the site that allows guest access will then be searchable on Google. In addition, people coming in to your site via a Google search will automatically be logged in as a guest.

**Profile visible roles**
Any role which is checked/ticked here will be visible on user profiles and the Participation screen. 

**Maximum uploaded file size**
Upload file sizes are restricted in a number of ways - each one in this list restricts the following ones:

1. The Apache server setting LimitRequestBody ... default in Apache 2.x or greater is set to 0 or an unlimited upload size

2. The PHP site settings post_max_size and upload_max_filesize in php.ini : modify php.ini in web server directories ( apache2.x.x/bin/php.ini ) not in php directories :
 
      post_max_size = 128M;  to increase limit to 128 Megabytes;
      upload_max_filesize = 128M;  to increase limit to 128 Megabytes;
      max_execution_time = 600 ; Maximum execution time of each script, in seconds;

3. The Moodle site-wide maximum uploaded file size setting: Settings > Site administration > Security > Site policies > Maximum uploaded file size.

4. The Moodle course maximum uploaded file size setting in the course default settings: Settings > Site administration > Courses > Course default settings

5. The file size settings in each individual course in Course Administration>Settings.

5. Certain course activity module settings (for example, Assignment) 

**User quota**
The maximum number of bytes that a user can store in their own Private files area.

**Allow EMBED and OBJECT tags**
Allowing these presents a security risk but if you wish normal users such as students to be able to use them then check the box here. 













