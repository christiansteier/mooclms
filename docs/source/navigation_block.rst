.. _navigation_block:

Navigation block
=================
The navigation block appears on every page of the site. It contains an expanding tree menu which includes My Home, Site Pages, My Profile, and Courses. What appears in the navigation block depends on the role of the user, where they are in the Moodle site, and any settings that have been applied globally. 

Overview
---------
The navigation block has links which can be expanded or collapsed.When logged in, a regular user will see the following as default: 

 * **My home** - This takes the user directly to their personal dashboard, :ref:`My home <my_home>`.

 * **Site pages** - This expands to show pages and resources available site wide, for example, user blogs and a calendar. Any items which have been added to the front page, such as resources/activities from the Main Menu block, or the Site News will also appear here. Other items depend on the role of the user, so an administrator will see reports and notes, for instance. 
 
 * **My profile** - This expands to allow regular users to view (and, if allowed, edit) their profile, view their forum posts, view and add and blog entries and messages and access their private files, providing these features have been enabled by the administrator. The administrator will also have a link here to Notes and Activity reports. 
 
 * **My courses** - This takes the user to their My Home page where they see the courses they are enrolled in. An administrator sees this link as "Courses", which expands to the course categories.
 
Navigation inside a course
^^^^^^^^^^^^^^^^^^^^^^^^^^^
 * **Current course** - When user is in a course, this link expands to show each section of the current course and any activities/resources which are in that section. 
 
 * **My courses** - When a non-admin user clicks this link in a course, it takes them to their :ref:`My home <my_home>` page where they will see other courses they are enrolled in. 
 
 * **Courses** - If the administrator has enabled "show all courses" in *Administration > Site administration > Appearance > Navigation*, then clicking on this link in a course will take the user to the courses index page course/index.php. 
 
Navigation block settings
--------------------------
An administrator can change navigation settings, such as the default home page, and whether to show course categories in the navigation, in *Settings > Site administration > Appearance > Navigation*. See :ref:`Navigation <navigation>` for details. 

Hiding the navigation block
-----------------------------
  * One way to make it harder for students to see other courses they are not enrolled in, is to implement the My Moodle page, and then hide the navigation block.
  * This will push all users to the My page on login, where they will see a list of those courses that they are enrolled in.
  * Hiding the navigation block will make it harder for them to find the other courses. 
 
