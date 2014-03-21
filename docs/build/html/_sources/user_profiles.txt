.. _user_profiles:

User Profiles
==============
A user's profile may be viewed by clicking on their name. See :ref:`View profile <view_profile>` for more information on how the profile information is displayed and :ref:`Edit profile <edit_profile>` for information on updating profiles. 

Site administration settings
------------------------------

Site policies
^^^^^^^^^^^^^^^
An administrator can force users to login for profiles and select which roles are visible in user profiles (by default teacher, non-editing teacher and student) in *Administration > Site administration > Security > Site policies*.

Default profile page
^^^^^^^^^^^^^^^^^^^^^
An administrator or manager (or any other user with the capability moodle/user:managesyspages) can set which blocks appear on the default profile page for new users.

 1. Access Administration > Site administration > Appearance > Default profile page.
 2. Select the required blocks from the "Add a block" drop-down menu. Configure each block as desired.
 3. Reposition blocks using the arrow icons in the block headers. 
 
Adding a block to all profile pages
-------------------------------------
An administrator can add a new block to all profile pages as follows:

 1. Turn editing on for the front page
 2. Add the block to the front page
 3. Edit where the block appears and set the page contexts to 'Display throughout the entire site'
 4. Go to your profile page and again edit where the block appears and set 'Display on page types' to 'Only user profile pages'.
 
Preventing users from customizing their profile page
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
By default, users can customize their public profile page and add blocks. To prevent this

 1. Go to *Administration > Site administration > Users > Permissions > Define roles*
 2. Edit the authenticated user role and untick the capability moodle/user:manageownblocks 
 
User profile capabilities
---------------------------
System:

 * Edit own user profile
 * Manage blocks on own public user profile
 * Configure default page layout for public user profiles
 * Update user profiles 

Users:

 * Edit user profile
 * Manage blocks on user profile of other users
 * View user full information 

Course:

 * View user profiles 





