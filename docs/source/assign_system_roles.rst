.. _assign_system_roles:

Assign System Roles
====================
You are here *Administration > Site Administration > Users > Permissions > Assign System Roles* .

In Moodle users do not normally have a global, site-wide role. In other words in Moodle you may have a teacher role in the course you teach in but a studentrole in another course.

Role assignment is within a defined context - for example site and course. When you create a new role or edit a pre-existing role via *Site Administration > Users > Permissions > Define roles*, you are asked in which context(s) you want the role to be assigned.

System context
^^^^^^^^^^^^^^^
   * *Administration > Site Administration > Users > Permissions > Assign system roles*
   * Any roles assigned here apply to the whole Moodle site. 

Front page context
^^^^^^^^^^^^^^^^^^^
   * *Administration > Site Administration > Front Page > Users > Permissions > Assigned roles*
   * Those with a role in the system context do not need to be assigned a role here as well.
   * However you might want to allow a teacher to manage items on the front page; in this instance, you would assign them the role on the Front page. 
   
Course Category context
^^^^^^^^^^^^^^^^^^^^^^^^
    * See Category enrolments
    * Users may be enrolled in the category to save enrolling them in each individual course in that category. 
    
Course context
^^^^^^^^^^^^^^^
    * *Go to Administration > Course administration > Enrolled users*
    * Click the "Enrol users" button and click those users you wish to enrol 

The dropdown menu at the top shows roles for which you are allowed to enrol; typically those users with lower roles than you.

Block context
^^^^^^^^^^^^^^
    * (Within the block) *Administration > Assign roles*
    * You may wish to assign roles to a block if, for instance you want specific people to see the block but for it to be hidden from others 

Activity Module context
^^^^^^^^^^^^^^^^^^^^^^^^
    * (Within the activity settings) *Administration > Locally assigned roles*
    * An example of this is assigning a student the teacher role locally in an individual activity like a forum so they can moderate their classmates' posts while still retaining the student role in the rest of the course. 

User context
^^^^^^^^^^^^^
    * The most common use of this is for the Parent role.
    * When the Parent role is created via *Administration > Site administration > Users > Permissions > Define roles* the "user" context box is checked.
    * To assign a parent the role in the context of their child (so they can see their child's grades etc) click the child's profile and then go to *Administration > Roles > Assign roles* relative to this user 

Hierarchy
^^^^^^^^^^
By assigning a role to a user in a certain context, you grant them the permissions contained in that role for the current context and all lower contexts.

The list of contexts in hierarchical order is as follows:

    * System (no parent)
    * Front page (parent = system) -
    * Course category (parent = parent category or system)
    * Course (parent = category or system)
    * Module (parent = course or system)
    * Block (parent = course or system)
    * User (parent = system) 

Roles can be inherited. For example if a user is assigned a Teacher role in a specific course category then the user will have this role in ALL courses within the category. Tip: use the override feature in a specific context for exceptions.

Roles will only work if the role assignment is made in the correct context. Some examples: a Teacher role should be assigned to a user in the course or course category context, a Forum moderator for a particular forum should be assigned in that specific forum. 

Hidden roles
^^^^^^^^^^^^^
If you want to provide users with access to the course, but don't want them to be visible in the participants list, use the Other users link in the course administration menu (*Administration > Course Administration > Users > Other Users*). Assigning roles here provides course access, and editing rights according to the permissions set for the role assigned without actually enrolling the user in the course. This is similar to the functionality of the "hidden user" check box in previous versions of Moodle. 


