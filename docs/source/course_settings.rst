.. _course_settings:

Course Settings
================
A teacher, or other user with the update course settings capability, can change course settings in *Administration > Course administration > Edit settings*. 

General
--------

.. image:: _images/course_general.png

Course full name
^^^^^^^^^^^^^^^^^^
This is the name of the course. It is displayed as a link on course lists on the Front page and on My home and in reports. It is also used in the browser title bar when the course is viewed.

The capability moodle/course:changefullname controls whether a user can edit the course full name. 

Short name
^^^^^^^^^^^
Many institutions have a shorthand way of referring to a course, such as BP102 or COMMS. Even if you do not already have such a name for your course, make one up here. It will be used in several places where the long name is not appropriate, such as the Navigation block.

The capability moodle/course:changeshortname controls whether a user can edit the short name field.

By default, only course full names are displayed in the list of courses. However an administrator can enable short names to be displayed too if required by ticking the checkbox in *Administration > Site administration > Appearance > Courses*.

Course category
^^^^^^^^^^^^^^^^
The site administrator may have created course categories to help teachers and students find their courses easily. Course categories may be reflected in the Navigation block.

The capability moodle/course:changecategory controls whether a user can edit the course category. 

Course start date
^^^^^^^^^^^^^^^^^^
This setting affects the display of logs and the weekly format topic dates.

If you use the "Weekly" course format, the start date will appear in the first section of the course. For example selecting 27 July, will display "27 July - 2 August" in the first section (when default display is selected for that section). 

This setting will not affect courses using the 'social' or 'topics' formats.

**TIP:** 1. If your institution runs on a weekly schedule, you may want to consider setting the start date for courses on the first day of the week, like a Monday. Please note that the 'first day of the week' is set by the langconfig file of your Language, and might be different from the default Monday of the English language pack. 

         2. In general, if your course does not have a real starting date then set the date to yesterday and use the availability setting to reveal the course to students. 

         3. See self enrolment course settings to prevent students from entering the course before a certain date/time. 

Viisible
^^^^^^^^^
Here you can "hide" your course completely. It will not appear on any course listings, except for managers, course creators, teachers and any other users with the view hidden courses capability. Even if students try to access the course URL directly, they will not be allowed to enter.

The hide/show courses capability controls whether a user can hide a course. 

Course ID number
^^^^^^^^^^^^^^^^^^
The ID number is an alphanumeric field. It has several potential uses. Generally, it is not displayed to students. However, it can be used to match this course against an external system's ID, as your course catalogue ID or can be used in the certificate module as a printed field.

The capability moodle/course:changeidnumber controls whether a user can edit the ID number. 



Description
-------------

.. image:: _images/course_description.png

Course summary
^^^^^^^^^^^^^^^
The summary appears on the course listings page. This field is searched when searching for a course and also appears in the Course/Site description block.

The capability moodle/course:changesummary controls whether a user can edit the course summary. 

Course summary files
^^^^^^^^^^^^^^^^^^^^^
An image (and if allowed by the administrator, other file types) may be attached to the course summary. They will be accessible by anyone from outside of the course just like the course name and/or summary.

By default, only jpg, gif and png file types are allowed as course summary files. An administrator can change the allowed file types in *Administration > Site administration > Appearance > Courses*. 









