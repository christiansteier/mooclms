.. _flat_file:

Flat file
==========
**Location:** Flat file edit settings link in *Administration > Site administration > Plugins > Enrolments > Manage enrol plugins*

A flat file allows bulk enrolment management (enrol or unenrol) of existing users in existing course. The file is read one time by Moodle then erased. The file is located in the moodle file structure as a text file and Cron provides the timing when it is read


Site setting for flat file enrolment
--------------------------------------
The site administrator should edit the settings for a flat file if it is enabled. 

You should specify an absolute path for the upload file (eg /var/moodledata/enrolments.txt) where it can be read and modified by the webserver process.

You can choose to have an email sent to notify the Administrator, Teachers and/or students when the file has been processed. 


Flat fle structure
--------------------
The file should be structured with the action, role, user id, and course ID number. Optionally a start time and end time can be added as additional fields.

Example file:

       add, student, 5, CF101
       add, teacher, 6, CF101
       add, teacheredit, 7, CF101
       del, student, 8, CF101
       del, student, 17, CF101
       add, student, 21, CF101, 1091115000, 1091215000

