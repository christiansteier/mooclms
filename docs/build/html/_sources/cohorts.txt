.. _cohorts:

Cohorts
========

Cohorts, or site wide cohorts, enable all members of a cohort to be enrolled in a course in one action, either manually or synchronised automatically.

Creating a cohort
^^^^^^^^^^^^^^^^^^
Cohorts can be created by site administrators and other users with appropriate permissions.

    1. Access Administration > Site administration > Users > Accounts > Cohorts
    2. Click the Add button
    3. NOTE In the dropdown you can choose between making your cohort available throughout the site "system" or in a named category.
    4. Complete the details and save the changes.
    5. Follow the assign link opposite the cohort name in the list of available cohorts.
    6. Select potential users from the list then click the Add button.

To synchronise cohort members with course participants, the Cohort sync enrolment plugin should be enabled in Administration > Site administration > Plugins > Enrolments > Manage enrol plugins.

Adding users to a cohort in bulk
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    1. Access Administration > Site administration > Users > Accounts > Bulk user actions
    2. Find users by setting an appropriate filter
    3. Add users from the available list to the selected list
    4. Choose 'Add to cohort' with selected users

Uploading users to a cohort
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
An administrator can upload users via CSV file to existing cohorts as follows:

     1. Access Administration > Site administration > Users > Accounts > Upload users

     2. Upload a text file with the following format:

.. list-table:: Cohort
   :widths: 20 20 20 20 20 20
   :header-rows: 1

   * - username
     - password
     - firstname
     - lastname
     - email
     - cohort1
   * - john
     - user*123
     - John
     - Teacher
     - john@example.com
     - first
   * - tanisha
     - user*123
     - Tanisha
     - Student
     - tanisha@example.com
     - second

Where first and second are the cohort ids of existing cohorts not their names.

Searching cohorts
^^^^^^^^^^^^^^^^^^
When a site has a large number of cohorts, keywords may be enetered into the search cohort box to search for the available cohorts.

Managing category cohorts
^^^^^^^^^^^^^^^^^^^^^^^^^^
Cohorts which have been created for a category rather than the system can be located by selecting the appropriate category and then clicking the Cohorts link in Administration > Category (name) > Cohorts.
