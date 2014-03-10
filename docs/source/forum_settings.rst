.. _forum_settings:

Forum
======
The forum module has additional settings which may be changed by an administrator in Administration > Site administration > Plugins > Activity modules > Forum and, for 'Maximum time to edit posts', in *Administration > Site administration > Security > Site policies*.

Use email address in reply
^^^^^^^^^^^^^^^^^^^^^^^^^^^
By default, a user's email is set as the 'From' address for forum notifications (unless the user has hidden their email address in their profile) so that recipients can choose to reply personally rather than via the forum. To set noreply@yourmoodlesite.org as 'From' address for all forum notification emails, untick the forum_replytouser checkbox. 

Long and short posts
^^^^^^^^^^^^^^^^^^^^^
The long and short post setting determine how forum posts on the site front page, social format course pages, and user profiles are displayed.

Enabling timed posts
^^^^^^^^^^^^^^^^^^^^^
Timed forum posts may be enabled i.e. having the option to set a display start and end date for a new discussion. Timed posts can then be created by users with the capability to view hidden timed posts (normally admins and teachers). 

Maximum time to edit posts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
This specifies the amount of time people have to re-edit forum postings, glossary comments etc. Usually 30 minutes is a good value. The setting may be changed by an administrator in *Administration > Site administration > Security > Site policies*.

Read tracking 
^^^^^^^^^^^^^^^
Sets the default 'Read tracking' selection when creating new forums. If 'Forced' is selected, the 'Allow forced read tracking' checkbox (below) must be ticked, otherwise 'Optional' will be the default setting. 

Allow forced read tracking
^^^^^^^^^^^^^^^^^^^^^^^^^^^
With this option set, "Forced" will be an option for "Read tracking" when creating or editing Forums. Forced forums have read tracking enabled regardless of user preference.

This setting can place additional load on servers. With this setting disabled, users who set their profile setting to not track read posts see faster load times of courses pages. With this setting enabled, that performance increase is lost, and all course views see the same performance as if the users personal setting was on.

When disabled, any forums previously set to "Forced" (or "On" prior to Moodle 2.6) will be treated as optional. 

Mark post read after 'X' days
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
This setting is forum_oldpostdays and specifies the number of days after which any post is considered to be read. E.g. If this is set to 14 days then any post older than 14 days will be considered read. If you set this to 0 then ALL posts are instantly considered to be read. If you don't want any posts to be considered read without the user reading them then set a high figure (e.g. 1000) 





