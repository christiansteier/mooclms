.. _theme_settings:

Theme Settings
===============
An administrator can change theme settings in *Settings > Site administration > Appearance > Themes > Theme settings*. 

Theme list
^^^^^^^^^^^
This lists the themes available for course and user themes. Leave this blank to allow any valid theme to be used. If you want to shorten the theme menu, you may specify a comma-separated list of names, though don't use spaces (e.g. standard,orangewhite).

You can preview the available themes in *Administration > Site Administration > Appearance > Themes > Themes selector*. 

Theme designer mode
^^^^^^^^^^^^^^^^^^^^^
Turn this on if you are designing and testing themes as it will stop the themes being cached and enable you to see theme changes quickly. (You can also do this with the Clear theme cache button on the theme selector page.)

Allow user themes
^^^^^^^^^^^^^^^^^^^
If the option allowuserthemes is enabled, each user may select their preferred theme on the edit profile page. All Moodle pages will be displayed in the user's theme, apart from courses where a course theme has been set.

**NOTE:** the user's theme will not be available in mobile and tablet devices unless the option enabledevicedetection is unchecked. 

Allow course themes
^^^^^^^^^^^^^^^^^^^^^
If you enable this, then teachers will be able to set their own course themes. Course themes override all other theme choices (site, user, or session themes).

   * If the option allowcoursethemes is enabled, each editing teacher may select their course theme via the Force theme option on the Course settings page. The course will always be displayed in the theme specified in the course setting, with user and the site themes being overwritten. 

**NOTE:** the course theme will not be available in mobile and tablet devices unless the option enabledevicedetection is unchecked.

Allow category themes
^^^^^^^^^^^^^^^^^^^^^^^
When enabled, themes can be set at the category level. This will affect all child categories and courses unless they have specifically set their own theme. WARNING: Enabling category themes may affect performance, as it will result in a few extra DB queries on each page, so only turn this on if you need it!

**NOTE:** the category theme will not be available in mobile and tablet devices unless the option enabledevicedetection is unchecked. 

Allow theme changes in the URL
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If this is checked then the theme may be changed by adding ?theme=theme_name (or &theme=theme_name if there are other URL parameters) to the URL in the browser. Theme names should be in lower case with spaces replaced by underscores, for example the theme "Formal white" should be entered as ?theme=formal_white .

Allow users to hide blocks
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Allows users to display and hide blocks.

Allow blocks to use the docks
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If the theme allows it, then checking this will allow the user to move blocks to the side dock. 

Custom menu items
^^^^^^^^^^^^^^^^^^^
The custommenuitems setting allows you to create a drop down menu that can be displayed by themes that support it. Currently all themes that are provided with Moodle 2.0 support this custom menu. 

The content of each item is constructed of up to three bits, each separated by a | (Shift + \) character. The bits are label | url | tooltip.

   * label - This is the text that will be shown within the menu item. You must specify a label for every item on the menu. 
   * url - This is the URL that the user will be taken to it they click the menu item. This is optional, if not provided then the item will not link anywhere. 
   * tooltip - If you provide a URL you can also choose to provide a tooltip for the link that is created with the URL. This is optional and if not set the label is used as the tooltip for the menu item. 

**Note:** The custom menu does not escape characters within the label, if you want to use a special HTML character such as an ampersand you must escape it yourself within the label. e.g. use & instead of &. 

Enable device detection
^^^^^^^^^^^^^^^^^^^^^^^^^
Will detect mobile and tablets that identify themselves via the web browser at the time of login to Moodle. These work with the theme selector. When the theme selector has identified a default, mobile and tablet themes, this feature will use that theme. 

Device detection regular expressions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
This will allow you to customize the theme selector options. For example, you can add a custom theme for IE6 and another for Windows CE by entering the identifying expressions the browser sends and the "Return value" you want to display as the theme selectors "Device type". 




Particular Theme Settings
---------------------------
Logo, tagline, link colour, column width, custom CSS and other settings for a particular theme may be set by an administrator in Administration > Site administration > Appearance > Themes > Theme name. 








