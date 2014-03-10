.. _scorm_settings:

SCORM
======
These options are available to the site admin in the Settings menu: *Site administration > Plugins > Activity Modules > SCORM Package*.

Default Value Settings
^^^^^^^^^^^^^^^^^^^^^^^
Many of the settings available in the SCORM Package administration simply set the default value for the SCORM activity module setup options provided within courses. Edit these settings to save yourself time when adding large numbers of packages, or to establish a standard for presentation across the site. 

Other Important Settings
^^^^^^^^^^^^^^^^^^^^^^^^^
The following options provided which do not simply set a default value for the SCORM activity editing page view.

**Auto-update frequency** - If not using a standard SCORM package uploaded using the filepicker and the SCORM package is hosted outside your Moodle installation the option to auto-update the package will be available - you can elect to have the package updated on every entry to the package or daily via the Moodle cron. 

**Enable external package type** - If selected, presents a text field to paste a URL to a remote imsmanifest.xml (in an unzipped remote SCORM package), as well as the file picker option provided by default. Note that the content is played from the designated location, and not unpacked into the Moodle file system. So if the base url is different from your moodle url then browser security will block cross-domain communcation and no grades/tracking information will be passed back to Moodle. 

**Enable downloaded package type** - If selected, presents a text field to paste a URL to a remote package.zip SCORM package. Package is downloaded and unzipped into the Moodle file system. 

**Enable IMS package type** - Enables a package to be selected from within an IMS repository 

**Force users to enable JavaScript** - Since the SCORM API uses JavaScript to save data to Moodle, this is a great idea! 

**Activate API debug and tracing** (set the capture mask with apidebugmask) - Turns on debugging for SCORM activities. In Moodle 2 you no longer have to also turn on debugging in the developer options. 

**API debug capture mask** - .* will debug for admin user only: You can use the mask to enable debugging under certain conditions. For example, if you are logged in using the admin user (username admin) you can set the api mask to: admin.* Users not logged in as admin will not see the debugging log. The "Default" api mask is .* which translates roughly to everybody. 

**Enable direct AICC url** - Makes it easier to connect to externally hosted AICC content as the teacher doesn't have to create an AICC package and is able to link directly to the external AICC url. 

**Enable external AICC HACP** - The SCORM activity can also support external AICC HACP Communication where the AICC package is hosted on an external content providers site and passes back http requests directly from the external server instead of within the users web browser session - this is disabled by default. 
