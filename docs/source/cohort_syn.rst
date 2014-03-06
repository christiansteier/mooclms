.. _cohort_syn:

Cohort sync
============
Cohorts, or site-wide groups, enable all members of a cohort to be enrolled in a course in one action, either manually or synchronised automatically. 

Enrolling a cohort in a course
-------------------------------
In order to actually enrol users from a Cohort into courses the *Cohort-Sync* Enrollment plugin needs to be added to the enrollment methods for the course. The Administrator will first need to enable the *Cohort-Sync* enrolment plugin site wide (*Administration > Site administration > Plugins > Enrolments*) and then add it to the required Course: (*Administration> Course administration > Users > Enrolment Methods*).

At this stage the *Cohort-Sync* instance for the course is edited and the appropriate Cohort selected. The role to which the Cohort users are assigned is also selected at this point (typically Student). 


Adding a cohort to a group
----------------------------
The cohort members can be added to a pre-made group at this stage also if desired. If any members are added or removed from the cohort, they are automatically added or removed from the group. Note that such members cannot be unenrolled manually from the groups screen and that additionally, there is information about their cohort below their name on the group screen. 

Visiting the *Administration > Course administration > Users > Enrolled Users* page will show users enrolled via the Cohort-Sync plugin.

Note that, by default, a teacher cannot add this plugin to their course. It needs to be configured by an Administrator or a user with the Manager role. Also note, that the user should be a Manager on a site level, not on the category or course level, otherwise the user will not see the option. If you want the user with the Manager role on the category level to see this enrol option, then you must add some cohorts on the category level, not on the site level.

The required capabilities for setting up a cohort sync are:

    * moodle/course:enrolconfig in the course context
    * moodle/cohort:config in the course context
    * moodle/cohort:view in the same context as category 

The required capabilities for manually enrolling cohort members are:

    * the same as cohort sync 
    * enrol/manual:enrol in course context
    * moodle/course:enrolreview in course context 
    


















