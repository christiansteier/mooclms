.. _manage_repositories:

Manage repositories
====================

Enabling repositories
-----------------------
Repositories can be enabled by an administrator in *Administration > Site administration > Plugins > Repositories > Manage repositories*.

A repository plugin may be set to

    * Enabled and visible - appears in the file picker
    * Enabled and hidden
    * Disabled - default setting 

The order in which repositories are shown in the file picker may be set using the up and down arrows. 

Vocabulary
------------
**Repository plugin:** it is also called a repository type. It can be named Box.net, Flickr, Mahara, Youtube... Adding a plugin allow users to create instances of this plugin. Only instances are displayed into the file picker. Type only exist in order to let a Moodle administrator to deactivate/delete all instances of a type in one click. 

**Repository instance:** An instance is displayed into the file picker and it is the access point to an external repository. An instance can have specific settings (for example be linked to a personal account).

   * First case: when you add the plugin, an instance is automatically created and can not be edited. The Moodle administrator cannot change the instance name. The instance name displayed into the file picker will be exactly the same as the plugin name. For example Youtube, Box.net...
   * Second case: the plugin allow the Moodle administrator to add multiple instances. An instance has a name for example Flickr Public access to Martin account, Martin's Mahara...
     For this second case it is important to identify two different kind of instances: 

       1. Common instances: The instances set by Moodle administrator in these same administration pages will be available into any file picker.
       2. Private instance: A teacher can set some instances available only for a course, and an user can set some instances only available for himself. In order to set instances for a course the teacher will go to the course page, and in order to set instances for a personal use, a user will go on his profile page. An administrator cannot add/edit private instances from the administration pages. 
