Upgrading
=========

Upgrading from Moodle
----------------------
You can only upgrade to Moodle 2.6 from Moodle 2.2 or later. If upgrading from earlier versions, you must upgrade to 2.2 first .

**Check the requirements -** Check that your server meets all requirements for 2.6 in Administration > Site administration > Server > Environment.

**Before you upgrade your site for real -**  We advise that you test the upgrade first on a COPY of your production site, to make sure it works as you expect.

**Backup important data -** The three should be backed up:

    * Moodle software (For example, everything in server/htdocs/moodle)
    * Moodle uploaded files (For example, server/moodledata)
    * Moodle database (For example, your Postgres or MySQL database dump)

**Put your site into maintenance mode -** You should put it into maintenance mode to stop any non-admin users from logging in.

**Install the new Moodle Software -** Steps to follow:

    1. Move your old Moodle files to another location.
    2. Unzip the Moodle package there so that all new files are in the location the old fles used to be in on the server.
    3. Copy your old config.php back to the new moodle directory.
    4. If you have any custom plugins, themes, add-ons on your site you should add them to the new code tree now.

**Finishing The upgrade -** Last step to follow:

Enter the moodle URL in your browser.

Then go to Administration > Site administration > Notifications.

Moodle will automatically detect the new version and  file systems upgrades that are necessary. If there is anything it can't do itself then you will see messages telling you what you need to do.


Automatic Update Deployment
----------------------------
An administrator can enable updates deployment in Administration > Site Administration > Server > Update notifications. Then when updates are available, 'Install this update' buttons are shown on Plugins overview and Plugins check pages.

Assignment Upgrade Helper
--------------------------

**Assignment upgrade tool**

The Assignment upgrade tool is an administrator tool for upgrading assignments in Moodle 2.2 and older to the new assignment module in Moodle 2.3 onwards.
It is recommended that admins upgrade all existing assignments to use the new assignment module as soon as possible, then disable the old assignment module (called 'Assignment 2.2' in Moodle 2.3 onwards), to avoid the confusion of having two assignment modules.

**Upgrading assignments**

To upgrade existing assignments to use the new assignment module

    1. Go to Administration > Site Administration > Assignment Upgrade Helper.
    2. Click List assignments that have not been upgraded to display a list of assignments created in a previous version of Moodle. This page lists the assignments created with an older version of Moodle that have not been upgraded to the new assignment module in Moodle 2.3. Not all assignments can be upgraded - if they were created with a custom assignment subtype, then that subtype will need to be upgraded to the new assignment plugin format in order to complete the upgrade.
    3. Select the assignment(s) you wish to upgrade and click the Upgrade selected assignments button in the Batch operations box at the bottom of the screen. Or click the Upgrade all assignments button in the Batch operations box.
    4. Confirm by clicking Continue.

A confirmation screen will appear.

**Disabling the old assignment module**

Once all existing assignments have been upgraded, the old assignment module can be disabled.

    1. Go to Administration > Site administration > Plugins > Activity modules > Manage activities
    2. Hide the Assignments 2.2 module by clicking on the eye in the hide/show column

Teachers will then have only the new assignment module available for selection in the activity chooser.


Question Engine Upgrade Helper
-------------------------------
The question engine upgrade helper is an admin tool for sites which have been upgraded from a pre-Moodle 2.1 version. Moodle 2.1 onwards uses a new question engine.
A site administrator can run the question engine upgrade helper in Settings > Site administration > question engine upgrade helper.

**Note:** You can reset any quiz that has been converted and then re-do it, but you should only do that if you have a good reason to do so and you don't have to.



 
