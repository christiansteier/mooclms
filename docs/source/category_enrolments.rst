.. _category_enrolments:

Category enrolments
==================== 
The category enrolments plugin allows users to be enrolled in a category as opposed to individual courses. The plugin has to be enabled by the site administrator. The category enrolment plugin will synchronise any role assignments at category context with the capability enrol/category:synchronised set to allow.


Course Settings for category enrolment
----------------------------------------
    * Go to the category into which you wish to enrol users. **Note:** You need to have category rights (manager or administrator) 
    * In the *Administration* block,click Assign roles. The list of possible roles you can assign will appear: 
    
    
Admin settings for category enrolment
---------------------------------------
The category enrolment plugin may be enabled or disabled throughout the site in *Administration > Site administration > Plugins > Enrolments> Manage enrol plugins*.

Assigning teachers or students to a category
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    * By default, only managers and course creators can be assigned category-wide. If you want to add teachers or students then the site administrator needs to tick the "category" box in their role in *Administration > Site administration > Users > Permissions > Define roles*.
    * To ensure they will be automatically assigned as teachers/students in any new courses you make, the administrator needs to set to "allow" the capability enrol/category:synchronised for the role in question in *Administration > Site Administration > Users > Permissions > Define roles*. 
    
