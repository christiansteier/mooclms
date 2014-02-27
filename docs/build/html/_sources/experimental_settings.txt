.. _experimental_settings:

Experimental Settings
======================
An administrator can enable certain experimental features in *Settings > Site administration > Development > Experimental > Experimental settings*.

An experimental feature is defined as a feature which require additional testing and bug-fixing. 

Safe exam browser
------------------
The Safe Exam Browser can work with Moodle to control what a student can do when in Moodle. To use it, it must be enabled in Settings > Site administration > Development > Experimental > Experimental settings. This adds the choice 'Require Safe Exam Browser' to the 'Browser security' field on the quiz settings form.

The Safe Exam Browser is offered under a Mozilla Public License and uses C++ and JavaScript. 

Features
^^^^^^^^^
Safe Exam Browser is a customised web browser that must be downloaded and installed on the computer that the student uses to attempt the quiz. The restrictions placed on students are similar to those in pop-up window case, but because Safe Exam Browser is software running on the student's computer, it can do a much more effective job of restricting their actions. If you select this option:

    * Students will only be able to attempt the quiz if they are using Safe Exam Browser.
    * The browser window will be fullscreen (without any navigation elements).
    * The window cannot be closed until the test is submitted.
    * Shortcuts keys such as Win, Ctrl+Alt+Del, Alt+F4, F1, Ctrl+P, Printscreen, are disabled.
    * Copy and paste, and the context menu, are disabled.
    * Switching to other applications is disabled.
    * Surfing to other web sites is prohibited. 
    
    
Group members only
--------------------
It can be enabled by an administrator in *Administration > Site administration > Development > Experimental*. 

Assigning an activity to a grouping
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
To assign an activity to a particular grouping:

    1. On the edit activity page, expand "Common module settings".
    2. Ensure that the group mode is set to separate or visible groups.
    3. Select the grouping from the grouping dropdown menu.
    4. Check the "Available for group members only" checkbox
    5. Click the "Save changes" button at the bottom of the page. 

The name of the grouping will then appear in brackets after the activity name on the course page. 

**Note:** If a graded activity is assigned to a particular grouping only, it will still appear in the gradebook for all users unless gradebook categories are set up in a certain way.

**Note:** You cannot make an activity visible to only one group of students without first placing them into a grouping. 



Drag and drop upload of text/links
------------------------------------
Enable or disable the dragging and dropping of text and links onto a course page, alongside the dragging and dropping of files. Note that the dragging of text into Firefox or between different browsers is unreliable and may result in no data being uploaded, or corrupted text being uploaded.



CSS optimiser
---------------
A CSS optimiser may be enabled by an admin in *Settings > Site administration > Development > Experimental > Experimental settings*. The tool analyses and refactors CSS before caching it.

When enabled CSS will be run through an optimisation process before being cached. The optimiser processes the CSS removing duplicate rules and styles, as well as white space removable and reformatting. Please note turning this on at the same time as theme designer mode is awful for performance but will help theme designers create optimised CSS.



New backup format
-------------------
If you have large courses you may find it useful to turn on an experimental option, 'Enable new backup format' from *Administration > Site administration > Development > Experimental > Experimental settings* .

This option selects a different internal backup format. Without this option, you cannot back up courses larger than 4GB.

You can change this option at any time. Whatever the option is set to, restore works for both the old and new format. The option only affects newly-created backups.

When you use this option, backup files still have the .mbz extension and work the same way, but there are some differences:

    * There is no limit on total backup size. (We have tested with courses up to about 10GB.)
    * Files may be slightly smaller.
    * If you need to edit this type of backup file manually, you will need to rename the .mbz file to .tar.gz, instead of .zip. You may need to use different software to extract and recompress this type of file. We have tested using GNU tar on Windows and Linux. 


