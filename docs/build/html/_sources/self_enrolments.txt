.. _self_enrolments:

Self enrolments
================
Self enrolment is the method whereby users can choose to enrol themselves into a course, either immediately by clicking "enrol me in this course" or by typing in an enrolment key they have been given. The enrolment plugin needs to be enabled by the site admin in enrolment plugins and has to be enabled within the course. The manual enrolment plugin has to be enabled in the same course as well. 

Course settings for self enrolment
------------------------------------
Checking self enrolment is enabled
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
In a course, go to *Administration > Course administration > Users > Enrolment methods* and ensure the "eye" is opened for self enrolment. 

.. image:: _images/self_enrolment.png

Adding an enrolment key to a course
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If you wish only a certain group of users to self enrol (and not anyone) then you can set an enrolment key which you then tell them to use when they access the self-enrolment screen.

Adding a group enrolment key to a course
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If you wish your users to enrol themselves directly into a group in the course then you can set a group enrolment key which you then tell them to use when they access the self-enrolment screen.


The following settings may be changed by clicking the edit (hand/pen) icon to the right of the self-enrolment option in *Administration > Course administration > Users > Enrolment methods* : 

Setting the enrolment period
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Tick the "enable" box to the right of Enrolment period and then choose your dates. 

Enrolment duration
^^^^^^^^^^^^^^^^^^^
Set the amount of time a user enrolment is valid, starting with the moment the user enrols themselves. If disabled, the enrolment duration will be unlimited. 

Notifying users when their enrolment expires
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
It is possible also for students and/or teachers to be notified when enrolments expire by selecting either "Enroller only" or "Enroller and enrolled user" from the dropdown "Notify before enrolment expires" and a time in "Notification threshold". 

Editing individual enrolment times
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
It is possible to edit the date and hour of an individual's enrolment from *Administration > Course administration > Users > Enrolled users* by clicking the edit icon in the enrolment methods column for the user in question. This then brings up a screen where the date and time can be modified. 

Unenrolling students who haven't been active on the course
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Choose from the dropdown to the right of "Unenrol inactive after..." 

Deciding the maximum number of users in your course
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Type the maximum number of users you want in your course in "Max enrolled users". When this limit is reached, nobody will be able to self-enrol. If you leave the number at 0 then there will be no maximum number. 

Allowing only cohort members to self-enrol
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If you have cohorts set up, then you can restrict self enrolment to particular cohorts by selecting the name of the cohort from the drop down box, A member of the cohort can self-enrol as normal; whereas a non-member gets a message telling them they are not able to self-enrol. 

Sending a welcome message to new users
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If enabled, users receive the following message via email when they self-enrol in a course:

      Welcome to {Course name}
      If you have not done so already, you should edit your profile page so that we can learn more about you: {link to profile page}

If you want to send a different message, simply type it in the custom welcome message text box.

**Note:** An admin can customise the message for the whole site by editing the *welcometocoursetext* language string. See Language customization for further details. 


Admin settings
---------------
The self enrolment plugin may be enabled or disabled throughout the site in *Administration > Site administration > Plugins > Enrolments > Manage enrol plugins*.

Shared settings for all courses
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The page Administration > Site administration > Plugins > Enrolments > Self enrolment. contains options for defaults that admin can set:

    * Require an enrolment key - if this box is ticked then all courses with self-enrolment enabled will need to have an enrolment key. The setting won't save until the teacher adds a key - something to be aware of as this can cause confusion:)
    * Use password policy - tick this box if you want enrolment keys set by teachers to follow the password policy of the site.
    * Show hint - tick this box if you are prepared to allow the first letter of a key to be given as a "hint"
    * Enrolment expiration action - specifies what happens when user enrolments reach expiration date. Please note that option "Unenrol user from course" purges grades, group memberships, preferences and other user related data from the courses.
    * Hour to send enrolment expiry notifications - specify hour for sending expiration notifications. 

Default enrolment settings in new courses
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
These can be set in Administration > Site administration > Plugins > Enrolments > Self enrolment but teachers in individual courses can alter them to suit their needs:

    * Add instance to new courses - if admin selects this, then any new course created will include the self enrolment plugin
    * Enable self enrolments- if this is enabled then users by default can self enrol into a course.
    * Use group enrolment keys - the setting for group enrolment keys in a course will be set to "yes" by default
    * Default role assignment - normally, when users self enrol, they have the student role. If necessary that role can be changed by default here - for example - if your Moodle has a dedicated role you wish to use instead.
    * Enrolment duration - this sets the default enrolment length for new courses (but again, may be altered by the course teacher.)
    * Notify before enrolment expires - specifies if teacher or optionally students should be notified before the expiration.
    * Notification threshold - specify how many days should be users notified before the enrolment expiration.
    * Unenrol inactive after- this sets the default time after which a student will be unenrolled if they haven't accessed the courses. (Teachers may change this)
    * Max enrolled users - adding a number here will specify the maximum number of users who can self-enrol into new courses. Teachers in the course can change this. If it is left at 0, there will be no maximum.
    * Send course welcome message- if this box is checked then newly enrolled users will receive a welcome message by default. 


Self enrolment method options
-------------------------------
One course may contain multiple self enrolment methods. User may be enrolled once in each instance only.

    * Custom instance name - specify custom enrolment method name.
    * Enable existing enrolments - if disabled all users enrolled via this plugin can not access course.
    * Allow new enrolments - disable if you do not want to allow students to self enrol in the future.
    * Enrolment key - specify key required for enrolment.
    * Use group enrolment keys - optionally use group keys for enrolment too.
    * Default assigned role - specify role to be assigned to suers during enrolment, this can be manually after user enrolment.
    * Enrolment duration - specify enrolment length, this can be manually after user enrolment.
    * Notify before enrolment expires - specifies if teacher or optionally students should be notified before the expiration.
    * Notification threshold - specify how many days should be users notified before the enrolment expiration.
    * Unenrol inactive after- specify time after which a student will be unenrolled if they haven't accessed the courses.
    * Max enrolled users - adding a number here will specify the maximum number of users who can self-enrol into this course.
    * Only cohort members - optionally restrict this enrolment method to members of specified cohort.
    * Send course welcome message- if this box is checked then newly enrolled users will receive a welcome message by default.
    * Custom welcome message - specify custom message if necessary. 













