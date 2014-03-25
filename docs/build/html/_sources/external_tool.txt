.. _external_tool:

External tool
==============
The external tool enables Moodle users to interact with LTI-compliant learning resources and activities on other web sites. For instance, an external tool could provide access to a new activity type or learning materials from a publisher.

Adding a new external tool to a course
----------------------------------------
  1. With the editing turned on,in the section you wish to add your external tool, click the "Add an activity or resource" link (or, if not present, the "Add an activity" drop down menu )and choose *External tool*
  2. This will take you to the settings page titled "Adding a new external tool". All settings may expanded by clicking the "Expand all" link top right.
  3. If the external tool has not been configured by the administrator, you will need to have in advance the correct URL, consumer key and secret. These should have been provided to you by the managers of the LTI compliant website you are going to be connecting to. Click "Show more" to access the consumer key and secret fields. 

General settings
^^^^^^^^^^^^^^^^^^

  .. image:: _images/external_tool1.png

 * **Activity name** - give the title you wish the students to see on the course page
 * **External tool type** - this is how Moodle communicates with the tool provider. If in doubt, leave as default. If your administrator has made a tool available sitewide, you will be able to select it here.
 * **Launch URL** - This is the URL for connecting to site.
 * **Launch container** - this is how the external tool will be displayed.
      
      * Default -if in doubt; leave as default
      * Embed - the external tool will be embedded in the Moodle course page with blocks and navigation bar
      * Embed without blocks - the external tool will be embedded in the Moodle course page but without blocks
      * New Window - the external tool will open in a new window. (A new window or tab will open with the External tool and the old browser window containing the course page will not change.) 

*The following settings are available by clicking ""Show more":*

 * **Activity description** - give a short description here
 * **Display description on course page** - choose to show the description along with the activity name
 * **Display activity name when launched** - have this appear when the student clicks the link.
 * **Display activity description when launched** - have this appear when the student clicks the link.
 * **Secure launch URL**
 * **Consumer key** -this tells the connecting LTI compliant site that your Moodle is allowed to connect. The "tool provider", ie the manger of the connecting LTI compliant site will issue you with this key. If you are merely linking to a tool with no secure access or gradebook sharing then you won't need a consumer key.
 * **Shared secret** - this is the "password" to connect to the tool - the LTI compliant site.
 * **Custom parameters** - most times you can leave this blank. The tool provider might use this to allow you to display a specific resource.
 * **Icon URL** - you can display a different icon from the default External Tool icon by entering its URL here
 * **Secure Icon URL** - enter the URL of a different icon here if your students are accessing Moodle securely via SSL. 
 
Privacy settings
------------------
(These settings are collapsed by default) 

  .. image:: _images/external_tool2.png

  * **Share launcher's name with the tool** - this means that the student's name will be displayed on the connected site as in this example
  * **Share launcher's email with the tool** - this means that the student's email will be displayed on the connected site as in this example
  * **Accept grades from the tool** - if this is checked, the connecting site will send back grades to Moodle's gradebook. See Using External tool for more information on this. 

Common module settings
------------------------
See :ref:`Common module settings <common_module_settings>`

Restrict access / Activity completion
---------------------------------------
(These settings are collapsed by default)

These settings are visible if :ref:`Conditional activities <conditional_activities_settings>`and :ref:`Activity completion <activity_completion_settings>` have been enabled in the site and the course. 

External tool capabilities
----------------------------
  * Add external tool
  * Submit a tool to admins for configuration
  * Grade external tool activities
  * Edit external tool activities
  * View external tool activities
  * Add a new external tool activity 

Why use an external tool?
---------------------------
  * Many websites provide materials and interactive learning excercises different from and complementary to Moodle's own resources and activities. The External tool module offers a way for teachers to link to these activities from within their Moodle course page and where available to have grades sent back into Moodle. Students only need to log in to Moodle; they do not have to log in a second time to the connecting site.
  * Sites which allow connection to Moodle in this way are known as LTI compliant and are called Tool providers. The "tools" are the exercises or materials which Moodle can connect to. 


