.. _upload_users:

Upload users
=============

An administrator can upload multiple user accounts via text file in *Administration > Site administration > Users > Accounts > Upload users*.

Upload user process
^^^^^^^^^^^^^^^^^^^^

Steps to be followed:

    * Create file for uploading.
    * Go to *Settings > Site administration > Users > Accounts > Upload users*
    * Add file to upload
    * Upload users preview - check settings and default user profile settings
    * Upload users preview - click "Upload users"
    * Upload users results - shows list of users, exceptions made in upload and summary of number of users
    * Upload users results - click "Continue"
    * Returns to Upload users screen

File formats for upload users file
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

You can use a spread sheet program to create the file with the required columns and fields. Then save the file as "CSV (comma delimited)". These files can be opened with simple text editors for verification.

File can include the following:

**Required fields :** username,firstname,lastname,email

Validity checks are performed for:

    1. username can only contain alphabetical lowercase letters , numbers, hypen '-', underscore '_', period '.', or at-sign '@'
    2. email is in the form: name@example.com .

**Password field :** "password" field is optional if "Create password if needed" setting is chosen (default).

    * If included, values should meet the requirements for the site's Password policy. To force password change for a particular user, set the password field to changeme.
    * If omitted, a password will be generated for each user (during the next Cron job) and welcome e-mails sent out.
    * Note: the text for the welcome e-mail is in the language settings. Please refer to this forum threadfor details.

**Optional fields :** To provide values other than the default include one or more of these

institution,department,city,country,lang,auth,timezone,idnumber,icq,phone1,phone2,address,url,description,mailformat,maildisplay,htmleditor,autosubscribe

**Additional name fields**

**Country :** use a country TWO LETTER CODE

**Custom profile field names :** (Optional). xxxxx is the real custom user profile field name (i.e. the unique shortname)

profile_field_xxxxx

**Special fields :** Used for changing of usernames or deleting of users

oldusername, deleted

**Enrolment fields** (Optional) : course1,type1,role1,group1,enrolperiod1,enrolstatus1/course2,type2,role2,group2,enrolperiod2/enrolstatus2 etc.

**Cohort field** (Optional) : cohort1

