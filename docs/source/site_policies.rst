.. _site_policies:

Site Policies
==============
 
Protect usernames
^^^^^^^^^^^^^^^^^^^^
If enabled, when a user attempts to reset their password and enters a username or email address, the following message is displayed: "If you supplied a correct username or email address then an email should have been sent to you." This is to prevent a malicious party from using the interface to determine which usernames and email addresses are in use in valid accounts.

If the protect usernames setting is disabled, when a user attempts to reset their password they are provided with feedback regarding whether an account exists with the username or email address supplied. For example, the message "The email address was not found in the database" may be displayed.

Force users to login
^^^^^^^^^^^^^^^^^^^^^^
If you turn this setting on, all users must login before they even see the Front Page of the site.

Force users to login for profiles
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Leave this set to Yes to keep anonymous visitors away from user profiles.

Force users to login to view user pictures
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If enabled, users must login in order to view user profile pictures and the default user picture will be used in all notification emails.

Open to Google
^^^^^^^^^^^^^^^
Enabling this setting allows Google's search spiders guest access to your site. Any part of the site that allows guest access will then be searchable on Google. In addition, people coming in to your site via a Google search will automatically be logged in as a guest.

Profile visible roles
^^^^^^^^^^^^^^^^^^^^^^
Any role which is checked/ticked here will be visible on user profiles and the Participation screen. 

Maximum uploaded file size
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

User quota
^^^^^^^^^^^^
The maximum number of bytes that a user can store in their own Private files area.

Allow EMBED and OBJECT tags
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Allowing these presents a security risk but if you wish normal users such as students to be able to use them then check the box here. 

Enable trusted content
^^^^^^^^^^^^^^^^^^^^^^^
By default Moodle will always thoroughly clean text that comes from users to remove any possible bad scripts, media etc that could be a security risk. The Trusted Content system is a way of giving particular users that you trust the ability to include these advanced features in their content without interference. To enable this system, you need to first enable this setting, and then grant the Trust submitted content capability to a specific Moodle role. Texts created or uploaded by such users will be marked as trusted and will not be cleaned before display

Maximum time to edit posts
^^^^^^^^^^^^^^^^^^^^^^^^^^^
This sets the editing time for forum postings. The editing time is the amount of time users have to change forum postings before they are mailed to subscribers. 

Full name format
^^^^^^^^^^^^^^^^^
This setting has been moved in Moodle 2.6 onwards to *Administration > Site administration > Users > Permissions > User policies*. 

Allow extended characters in usernames
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The default here, unchecked = unenabled, can only contain alphabetical letters in lowercase, numbers, hypen '-', underscore '_', period '.', or at sign '@'. If you enable this, it will be possible to have any characters for the username. 

Site policy URL
^^^^^^^^^^^^^^^^
    * If you have a site policy that all users must see and agree to before using this site, then specify the URL to it here, otherwise leave this field blank. The URL can point to any type of file anywhere online that can be accessed without a log in to your Moodle.
    * It is recommended that the site policy is on the same domain as Moodle to avoid the problem of Internet Explorer users seeing a blank screen when the site policy is on a different domain.
    * The site policy will be displayed in a frame. You can view it via the URL yourmoodlesite.org/user/policy.php. 

Site policy URL for guests
^^^^^^^^^^^^^^^^^^^^^^^^^^^
This is similar to the Site policy URL as above but will be seen by those to whom you give guest access. 

Keep tag name casing
^^^^^^^^^^^^^^^^^^^^^
If checked, then tags like the following will be displayed: SOCCER, gUiTaR, MacDonalds, music

If unchecked, then all tags will be displayed as follows: Soccer, Guitar, Macdonalds, Music 

Profiles for enrolled users only
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
To prevent misuse by spammers, profile descriptions of users who are not yet enrolled in any course are hidden. New users must enrol in at least one course before they can add a profile description.

Cron execution via command line only
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Cron is an action that runs various administrative jobs on your Moodle such as sending out forum posts. Normally Cron can be run by typing www.YOURMOODLE.com/admin/cron.php but as anyone logged in can do this, if you wish to prevent it, then check this box and only a admin can run Cron from the command line.

Cron password for remote access
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Setting a password here will mean that users can only run cron from the browser if they know the password and add it like this: www.YOURMOODLE.com/admin/cron.php/?password=THEPASSWORDYOUSET 

Account lockout
^^^^^^^^^^^^^^^^
In Moodle 2.5 onwards, account lockout may enabled. After a specified number of failed login attempts, a user's account is locked and they are sent an email containing a URL to unlock the account.

The account may also be unlocked by an administrator in *Settings > Site administration > Users > Accounts > Browse list of users* or by waiting for the account lockout duration to elapse. 

Password policy
^^^^^^^^^^^^^^^^
It is highly recommended that a password policy is set to force users to use stronger passwords that are less susceptible to being cracked by a intruder. 

Group enrolment key policy
^^^^^^^^^^^^^^^^^^^^^^^^^^^
If this is enabled then when a teacher sets a group enrolment key, they will have to set a key which follows the password policy set above.

Disable user profile images
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Check/tick this box if you don't want your users to be able to change their profile images. 

Email change confirmation
^^^^^^^^^^^^^^^^^^^^^^^^^^
A confirmation step is required for users to change their email address unless the *emailchangeconfirmation* box is unchecked. 

Remember username
^^^^^^^^^^^^^^^^^^
If you want usernames to be stored during login then set this to "yes". This will store permanent cookies and in some countries may be considered a privacy issue if used without consent

Strict validation of required fields
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If enabled, users are prevented from entering a space or line break only in required fields in forms.




