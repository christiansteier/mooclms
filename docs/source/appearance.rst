Appearance
===========
There are many ways to customise the appearance of your Moodle site so that it blends in with, for example, your college site or your company's corporate brand. Below links provide more information on personalising the appearance of Moodle:

Themes
-------




Calendar
----------




Blog
-----





Navigation
------------




HTML Settings
---------------





Media Embedding
-----------------





Moodle Docs
-------------


Moodle Docs is an abbreviation for *Moodle documentation*.

By default, managers, teachers and non-editing teachers (and any other users with the capability moodle/site:doclinks) have "Moodle Docs for this page" links at the bottom of each page in Moodle for accessing context-specific documentation.

An administrator can change Moodle Docs settings in *Settings > Site administration > Appearance > Moodle Docs*.

The default path is to docs.moodle.org. If a user has selected a language for which there is documentation available, the "Moodle Docs for this page" links will link to the documentation in that language.

If the Moodle Docs document root field is left blank, no "Moodle Docs for this page" links will appear.

You may find that teachers prefer the documentation to open in a new window, so they can easily return to their page in Moodle. If so, click the "Open in new window" checkbox. 



Default My home page
----------------------
An administrator or manager (or other user with the capability moodle/my:configsyspages) can set which content (course overview, calendar, blocks) appears on the My home page for new users as follows:

    1. Access *Settings > Site administration > Appearance > Default My Moodle page* .
    2. Select the required blocks from the "Add a block" drop-down menu. Configure each block as desired
    3. Reposition blocks using the arrow icons in the block headers 



Default profile page
----------------------
An administrator or manager (or any other user with the capability moodle/user:managesyspages) can set which blocks appear on the default profile page for new users.

    1. Access *Administration > Site administration > Appearance > Default profile page*.
    2. Select the required blocks from the "Add a block" drop-down menu. Configure each block as desired.
    3. Reposition blocks using the arrow icons in the block headers. 



Courses
---------
An administrator can change the following course settings in Settings > Site administration > Appearance > Courses.

   * Course contacts - Users with the selected role(s) e.g. teachers are listed in the course description. By default, users with the role of teacher in a course are listed in the course description for that course. If a course has several teachers, the course description can become rather long. In this case, you can create a role e.g. head of subject with no capabilities set and assign it to selected users in addition to their teacher role. If you then select only the head of subject role in the course managers setting, the course description will be shorter. 

   * Display extended corse names - By default, only course full names are displayed in the list of courses. If you check this box, then the course short name will also be displayed. 

   * Course per page - You can define value for the number of courses to be displayed per page in a course listing.
   
   * Courses with summaries limit - maximum number of courses to display in a course listing including summaries before falling back to a simpler listing.
   
   * Course summary files limit - The maximum number of files that can be attached to a course summary.
   
   * Course summary files extensions - A comma-separated list of allowed course summary files extensions.





Ajax and Javascript
---------------------
Admins can choose to disable AJAX across the whole site in *Settings > Site administration > Appearance > AJAX and Javascript*.

Ajax is required for drag and drop functionality so leaving it enabled is recommended. 



Manage Tags
-------------
Tags can be managed by a site administrator or manager (or any other user with the capability moodle/tag:manage) in Settings > Site administration > Appearance > Manage tags.

The manage tags page provides a list of tags, together with information on their creators, how many times they are used, when they were last modified and which tags have been flagged as inappropriate. Inappropriate tags are shown in red when using the default theme. 

Please see :ref:`tags` to know more about tags.



Additional HTML
-----------------
An administrator can add additional HTML to every page in *Settings > Site administration > Appearance > Additional HTML*.

These settings allow you to specify HTML that you want added to every page without altering the Moodle code files.

You can add HTML will be added within the HEAD tag for the page, immediately after the BODY tag has been opened, or immediately before the body tag is closed.

Doing this allows you add custom headers or footers on every page, or add support for services like Google Analytics very easily and independent of your chosen theme. 





