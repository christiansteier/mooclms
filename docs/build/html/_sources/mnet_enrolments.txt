.. _mnet_enrolments:

MNet remote enrolments
=======================
MNet remote enrolments allows a remote MNet host to enrol their users into our courses.

Setting up enrolments
-----------------------
Say I want administrators on 'Site A' to be able to enrol their users to courses 'Site B' I need to take the following steps. Note you need to set up Site B first before enrolling users to it.

Pre-requisites
^^^^^^^^^^^^^^^
    * At least 2 networked peers
    * Mnet Authentication plug-in enabled
    * Mnet Enrolment plug-in enabled 

Enabling a course for peer enrolments (Site B)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    * Go into the course that you want to enable on 'Site B'.
    * Go to *Administration > Course administration -> Enrolment Methods* and add an Mnet enrolment instance linked to 'Site A' 

Enrolling Users (Site A)
^^^^^^^^^^^^^^^^^^^^^^^^^
Note this will only work for system users with moodle/site:config capability

    * Go to *Networking -> Remote enrolment clients*
    * Choose Edit Enrolments in the action column for Site B
    * Select Edit Enrolments in the Action column of the appropriate course (use refresh if not there)
    * Enrol the relevant users 

Accessing the course
^^^^^^^^^^^^^^^^^^^^^^
The users that were enrolled will now have access to the remote site. the links will appear in the 'My Courses' area and 'Course Overview' block but not in the Navigation block under 'Courses'.

The get_my_remotecourses() function can be used to work with these elsewhere .

