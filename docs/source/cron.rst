.. _cron:

Cron
=====
The Moodle 'cron' process is a PHP script (part of the standard Moodle installation) that must be run regularly in the background. The Moodle cron script runs different tasks at differently scheduled intervals.

**IMPORTANT: Do not skip setting up the cron process on your server for your Moodle. Your site will not work properly without it**.

A special program (typically called - not surprisingly - 'cron') is used to run the Moodle cron script at a regular interval. The Moodle cron script runs tasks include sending mail, updating Moodle reports, RSS feeds, activity completions, posting forum messages and other tasks. Since different tasks have different schedules, not every task will run in Moodle when the cron script is triggered.

The cron program (that runs the Moodle script) is a core part of Unix based systems (including Linux and OSX) being used to run all manner of time-dependent services. On Windows the simplest solution is to create a task in the Windows Task Scheduler and set it to run at regular intervals. On shared hosting, you should find the documentation (or ask support) how cron is configured.

Essentially, the task involves adding a single command to the list of cron activities on your system. On Unix based systems this list is a file called a 'crontab' which all users have. 


Working out the Moodle cron command
-------------------------------------
Moodle has two different ways to deploy cron which use different scripts within the Moodle install. These are as follows...

   1. The CLI (command line interpreter) script. This will be at the path 
   
       /path/to/moodle/admin/cli/cron.php
   
      If in doubt, this is the correct script to use. This needs to be run by a 'PHP CLI' program on your computer. So the final command may look something like 
      
       /usr/bin/php /path/to/moodle/admin/cli/cron.php
       
       You can (and should) try this on your command line to see if it works. 
       
   2. The web based script. This needs to be run from a web browser and will be accessed via a web url something like http://your.moodle.site/admin/cron.php. You can find command line based web browser (e.g. wget) so the final command may look like 
   
       /usr/bin/wget http://your.moodle.site/admin/cron.php
       
       This has the advantage that it can be run from *anywhere*. If you can't get cron to work on your machine it can be run somewhere else. 
       
       
