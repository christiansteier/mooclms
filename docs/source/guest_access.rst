.. _guest_access:

Guest Access
=============
The Guest access plugin allows users with the Guest role to view the contents of a course. This might be used, for example, if a Moodle site serves as a website where certain courses contain publicly available information, or else with a commercial Moodle site where courses with guest access can offers a "taster" of the kind of courses which may be purchased. (Note that the guest cannot participate in any activities; they can only view content.) 


Course settings for guest access
---------------------------------
    * In *dministration > Course administration > Users > Enrolment methods*, first ensure that you have added "guest access" as an enrollment method, and that it has its eye open.
    * Ensure that self enrolment is also enabled.
    * In *Administration > Course administration > Edit settings*, scroll to "Guest access"
    * Set the drop down to "Yes"
    * If you wish guests to use a password to access the course then add it here.
    
Admin settings for guest access
---------------------------------
    * In *Administration > Site administration > Plugins > Enrolments > Manage enrol plugins*,ensure Guest access is enabled (has its eye open.) This enables Guest access.
    * In *Administration > Site administration > Plugins > Manage authentication* set the Guest login button to Show if you want the button on the Frontpage.
    * Also Guest accounts can be logged - check the *Administration> Site administration > Server > Cleanup > Log guest access* setting 
    
Default settings for guest access
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    * Clicking on *Administration > Site administration > Plugins > Enrolments > Guest access* brings up the screen where admin can set defaults for guest access in courses. Guest access can be turned on by default in all new courses and you can also:
        * require each course with guest access to have a password for guests. (Note: this can confuse teachers who are not aware of the requirement.)
        * use or ignore your Moodle's standard password policy for guest access passwords
        * offer if needed the first letter of the password as a hint. 
        
Auto-login guests
^^^^^^^^^^^^^^^^^^
    * In *Administration > Site administration > Users > Permissions > User policies8, you can tick the box so that visitors are automatically logged in as guests when accessing a course with guest access (i.e. they don't have to click the "login as guest button".
    * In *Administration > Site administration > Plugins > Authentication > Manage Authentication*, you must have "Guest login button" set to "Show".
    * In *Administration > Site administration > Security > Site policies* you can check "Open to Google" setting so that the Google search robot will be allowed to enter your site as a Guest. In addition, people coming in to your site via a Google search will automatically be logged in as a Guest. 

   
    
