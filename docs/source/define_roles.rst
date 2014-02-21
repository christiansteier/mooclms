.. _define_roles:

Define Roles
=============
A role is a collection of permissions defined for the whole system that you can assign to specific users in specific contexts. The combination of roles and context define a specific user's ability to do something on any page. The most common examples are the roles of student and teacher in the context of a course. 

For example, you may have a role called ‘Trainer’ set up to allow trainers to do certain things (and not others), once this role exists you can assign it to someone in a course to make them a ‘Trainer’ for that course. You could also assign the role to a user in the course category to make them a ‘Trainer’ for all the courses under that category, or assign the role to a user just in a single forum, giving that user those capabilities just in that forum. 

Defining User Roles
^^^^^^^^^^^^^^^^^^^^
The 'Define roles' page has three tabs: Manage roles, Allow role assignments and Allow role overrides.
 
The 'Manage roles' tab contains a list of roles on your site. The Edit column contains icons for editing and deleting roles, and for moving them up or down in the list (affecting the way that roles are listed around Totara). Below the table is an 'Add a new role' button.
 
If you wish to modify the capabilities for a particular role, you can do so by editing the role.
For example you may want to allow trainees to unenrol themselves from a course when using internal enrolment. 

Permissions
^^^^^^^^^^^^
You have three permission levels for each task:
 
**Allow:** The role is assigned in the stipulated context.
 
**Prevent:** By choosing this you are removing permission for this capability, even if the users with this role were allowed that permission in a higher context.
 
**Prohibit:** This is rarely needed, but occasionally you might want to completely deny permissions to a role in a way that can not be overridden at any lower context. A good example of when you might need this is when an admin wants to prohibit one person from starting new discussions in any forum on the whole site. In this case they can create a role with that capability set to ‘Prohibit’ and then assign it to that user in the site context. 

**Allow role assignments:** This defines what roles each of the roles listed can allocate to users in the site.
 
**Allow role overrides:** This defines what role permissions can be overridden by the roles on the left.
