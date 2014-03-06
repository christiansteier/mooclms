.. _course_metalink:

Course meta link
=================
The Course meta link plugin makes it possible for one course, called a metacourse, to bring in enrolments from other courses. The Course meta link plugin needs to be enabled both on the site level by the site admin and has to be enabled within the course. 

Metacourse examples
---------------------
**Examples:** one "child" course (a course linked to a meta course) can be associated with many meta courses. Or one meta course can have many child courses associated with it. Both the child courses (non-meta courses) and the meta courses are independent and can be recycled many times, that is, each can be associated with many of the other. 

Course settings for Course meta link
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    * In a course, go to *Administration > Course administration > Users > Enrolment methods*.
    * Click the dropdown menu under the enrolment methods and select 'Course meta link'. 
    * In the screen that comes up next, select from the dropdown box the course you wish to bring enrolments from and then click 'Add method'.
      
      Note 1: A teacher in a course will only be able to choose from courses they are teachers in elsewhere. 
      Note 2: To add more courses, add another instance of the course meta link. 
      
    * The users from the child course will now be enrolled in the current course.
    * When new users are enrolled to the child course, they will be automatically brought into the current metacourse. 

Site settings for Course meta link
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The Course meta link plugin may be enabled or disabled throughout the site in *Administration > Site administration > Plugins > Enrolments > Manage enrol plugins*.

The page *Administration > Site administration > Plugins > Enrolments > Course meta link* contains options for defaults that admin can set. (It can be also be accessed by clicking the Settings link on on the course meta link section of *Administration > Site administration > Plugins > Enrolments > Manage enrol plugins*)

By default all role assignments from child courses are synchronised to meta courses. However, the "Roles that are not synchronised to metacourses" setting enables administrators to exclude particular roles. 
  
Enabling teachers to add meta links
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
An administrator can enable teachers to add course meta links as follows:

    * Go to *Administration > Site Administration > Users > Permissions > Define Roles*
    * Select the Teacher Role and click on the Edit button
    * Scroll down to Course Meta Link.
    * Scroll to the bottom of the page to save your changes. 
    
