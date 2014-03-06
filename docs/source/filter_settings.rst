.. _filter_settings:

Common filter settings
=======================

A site administrator can change the following settings in Settings > Site administration > Filters > Common filter settings:

    * Text cache lifetime - Text filters can take a lot of processor power to analyse. If you have a large number of courses, the filters may slow your system. The text cache lifetime determines how often the filters run. If you set them to run too frequently, your system may slow down. If you set them to run too infrequently, analysing new content will take too long and users will notice. You should experiment to find the correct amount of time for your server.
    * Filter uploaded files - This setting enables uploaded files (HTML and text only) to be processed by the filters system. You can choose to have none, only HTML or all files filtered.
    * Filter match once per page - This setting effects the glossary, activity and resource linking filters. If set to yes, only the first match on the complete page will be converted to a link. All others will be ignored.
    * Filter match once per text - This setting effects the glossary, activity and resource linking filters. If set to yes, only the first match in a discrete block of text will be converted to a link. All others in that text block will be ignored.
    * Filter all strings - The filter all strings common filter setting in Moodle 1.9 (which only worked for the multi-language filter) has been replaced by the 'Apply to' setting in Manage filters. 

File activity module setting
------------------------------

A site administrator can change the following setting in Settings > Site administration > Plugins > Activity modules > File:

    * Use filters on file content - This applies to content in HTML pages.
