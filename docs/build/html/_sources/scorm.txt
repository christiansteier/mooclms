.. _scorm:

SCORM
======

The SCORM module enables you (the teacher) to upload any SCORM or AICC package to include in your course.

SCORM 1.2 is supported in Moodle but SCORM 2004 is not.

SCORM (Sharable Content Object Reference Model) is a collection of specifications that enable interoperability, accessibility and reusability of web-based learning content. SCORM content can be delivered to learners via any SCORM-compliant Learning Management System (LMS) using the same version of SCORM. 

Adding a SCORM package
------------------------
To add a SCORM package to your course

**Quick method:** (Note - does not work with versions of Internet Explorer earlier than IE10)

  1. Click the 'Turn editing on' button at the top right of the course page
  2. Drag and drop the SCORM package zip file onto the course section where you'd like it to appear
  3. Answer 'Add a SCORM package' to the popup dialogue asking what you want to do with the zip file then click the upload button
  4. If necessary, edit the title of the file by clicking the pencil icon, or edit other options (see below) by clicking the editing icon 

**Note:** It is currently not yet possible to add AICC packages using the quick method. 

**Longer method:**

  1. Click the 'Turn editing on' button at the top right of the course page
  2. Click the 'Add an activity or resource' link in the section you wish to add your SCORM package, then in the activity chooser, select SCORM package then click the Add button (or select 'SCORM package' from the 'Add an activity' dropdown menu)
  3. Enter a name and a description (which may be required or optional according to the admin settings)
  4. Either drag and drop a SCORM package zip file into the box with an arrow or click the Add button to open the File picker menu in order to choose a file from your computer or a repository
  5. Select display and other options as required (see below)
  6. Click the button 'Save and display' at the bottom of the page 

You can edit or update the SCORM package later by clicking on the edit icon (usually a hand/pen) or by clicking on its name and then Settings > SCORM/AICC administration > Edit settings. 

**Note:** Moodle does not generate SCORM content. Moodle presents the content in SCORM packages to learners, and saves data from learner interactions with the SCORM package

Scorm administration settings
-------------------------------

General
^^^^^^^^
 
**Name**

Whatever you type here will form the link learners click on to access the SCORM package, so it is helpful to give it a name that suggests its purpose.

**Description**

Add a description of your SCORM activity here. Click "Show editing tools" to display the rich text editor, and drag the bottom right of the text box out to expand it.

**Display description on the course page**

If this box is ticked, the description will appear on the course page just below the name of the SCORM activity.

**Package**

This setting determines which SCORM package is used by this SCORM activity. Drag and drop or click the icon top left to upload your SCORM package. (Note that you must not unzip the package before upload.)The default (1) is to be able to upload a file. If your admin has added additional options in Site administration>Plugins>Activity modules>SCORM package then these will be available in a dropdown menu. (2) 

**Alias/Shortcut**

If you access your SCORM package from a repository (such as File system repository or Private files) you can choose to create an alias/shortcut to it and then set an update frequency to set how often Moodle should check to see if there is an updated zip.

**Selecting an imsmanifest.xml**

It it possible to select the imsmanifest.xml file and have it as an alias/shortcut. To do this, you need to have created a File system repository and, when configuring it, allowed relative files. Extract your SCORM package into a folder there. When clicking on the Add button to add your SCORM package, select the file system repository folder with your SCORM package and browse for and select the imsmanfest.xml file, ensuring you the option to create an alias/shortcut to the file. Save and display.


**Note:** The settings (Type, URL and Auto-update frequency) are only available when configured globally.

Appearance
^^^^^^^^^^^
(These settings are collapsed by default) 

**Display package**

Choose from current or new window. Note that if you choose a new window, students need to ensure pop ups are enabled.

**Display course structure on entry page**

If this is enabled then the table of contents of the package will be displayed when the students clicks to access the package.

**Hide navigation buttons**

**Display attempt status**

You can choose whether to display a summary of the student's attempts on the entry page, on their My home page or both. This setting is helpful when debugging grading issues - working out why a user got a certain grade.

*The following settings become visible when "Show more" is clicked:*

**Width**

Stage size width as a css value, either % or pixels. Default is 100%. You can change to a different percentage by putting a % symbol after the number (ex. 80%). You can also set to a pixels value by entering a number higher than 100 (ex. 800).

**Height**

Stage size height as a css value, either % or pixels. Default is 500 pixels. You can change to a percentage by putting a % symbol after the number (ex. 80%). You can also set to a pixels value by entering a number higher than 100 (ex. 800).

**Options**

There is a series of check boxes for:Allow the window to be resized ad scrolled, displaying directory links, location bar, menu bar, toolbar and/or status.

  * **Student skip content structure page** - never, first access, always
  * **Disable preview mode** - If this option is set to Yes, the Preview button in the view page of a SCORM/AICC Package activity will be hidden. The student can choose to preview (browse mode) the activity or attempt it in the normal mode. When a Learning Object is completed in preview (browse) mode, it's marked with browsed icon
  * **Display course structure in player**
  
Availability
^^^^^^^^^^^^^
(These settings are collapsed by default.) 

Choose here the dates you wish the SCORM package to be available to students. 

Grade
^^^^^^
(These settings are collapsed by default) 

**Grading method**
    
  * **Learning Objects** - This mode shows the number of completed/passed Learning Objects for the activity. The max value is the number of Package's Learning Objects. Tip: If your SCORM package does report cmi.core.lesson_status, and does not report cmi.core.score.raw, then you should use this setting.
  * **Highest grade** - The grade page will display the highest score obtained by users in all passed Learning Objects. Tip: If your SCORM package does report cmi.core.score.raw, and does not report cmi.core.lesson_status, then you should use this setting, Average grade, or Sum grade.
  * **Average grade** - If you choose this mode Moodle will calculate the average of all scores.
  * **Sum grade** - With this mode all the scores will be added. 

**Maximum grade**

Not applicable if Grading Method is Learning objects. Usual setting is 100. If your SCO 's high score is something other than 100, you should adjust this value appropriately. When grading Method is one of the score settings, then the gradebook grade is package score divided by this number. 

Attempts management
^^^^^^^^^^^^^^^^^^^^
(These settings are collapsed by default.) 

**Number of attempts**

Defines the number of attempts permitted to users. It works only with SCORM 1.2 and AICC packages. SCORM2004 has its own max attempts definition.

  * The option to start a new attempt is provided by a checkbox above the Enter button on the content structure page, so be sure you're providing access to that page if you want to allow more than one attempt.
  * An attempt is not complete until the cmi.core.lesson_status for the attempt is set to either 'completed' or 'passed'. After that, the Start new attempt checkbox is available to the learner. 

**Attempts grading**

When you permit multiple attempts for students, you can choose how to record the result in gradebook by first, last, average or highest settings.

  * Display attempt status - If enabled, scores and grades for attempts are displayed on the SCORM outline page. This setting makes the block display more info to the user on the entry page to the SCORM and in the course overview block - if you turn it off it will display less info. This setting is helpful when debugging grading issues - working out why a user got a certain grade. 

**Force new attempt**

If this is enabled then every time the student accesses the package, it will count as a new attempt.

**Lock after final attempt**

If this is enabled then once a student has used up all their attempts, they can no longer access the SCORM package. 

Compatibility settings
^^^^^^^^^^^^^^^^^^^^^^^
(These settings are collapsed by default.) 

**Auto-Continue**

If Auto-continue is set to Yes, when a Learning Object calls the "close communication" method, the next available Learning Object is launched automatically.If it is set to No, the users must use the "Continue" button to go on.

**TIP:** Auto-Continue will only to move from one SCORM to the next in the same topic. 

**Force completed**

If this is enabled then the status of the current attempt is set to "complete". Note that this only applies to SCORM 1.2 packages and is useful if the SCORM package does not handle revisiting an attempt correctly, in review or browse mode, or otherwise incorrectly issues the completion status.

  * Auto-update frequency - If not using a standard SCORM package uploaded using the filepicker and the SCORM package is hosted outside your Moodle installation the option to auto-update the package will be available - you can elect to have the package updated on every entry to the package or daily via the Moodle cron. 

Common module settings
^^^^^^^^^^^^^^^^^^^^^^^
(These settings are collapsed by default.)

See :ref:`Common module settings <common_module_settings>`

Restrict access
^^^^^^^^^^^^^^^^
(These settings are collapsed by default)

These settings are visible if :ref:`Conditional activities <conditional_activities_settings>` have been enabled.

Activity completion settings
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If this has been enabled for the course, then SCORM completion may be set based on minimum score or status (e.g. "Passed"). 

As in most activities there are 3 save button choices. Cancel, Save and return to course and Save changes buttons. The Save changes button will take the teacher back to the SCORM "stage" page. 








