.. _upload_courses:

Upload courses
===============
To upload one or more courses

    1. Go to *Administration > Site administration > Courses > Upload courses*
    2. Either drag and drop the CSV file or click the 'Choose a file' button and select the file in the file picker
    3. Select appropriate import options carefully, then click the preview button. 
    
Note: It is also possible to use the command-line tool *admin/tool/uploadcourse/cli/uploadcourse.php*.

When using the web interface, use the Preview option to see if any errors were detected in the previewed rows. If you proceed with the upload and there were something wrong detected with a course, it will be ignored. 

Example: 
uploadcourse.csv :

.. list-table:: Cohort
   :widths: 20 20 20 20 20 20 20 20
   :header-rows: 1

   * - shortname
     - fullname
     - category
     - summary
     - enrolment_1
     - enrolment_1_role
     - enrolment_1_enrolperiod
     - role_student
   * - courserestored
     - Course restored
     - 1
     - a summary
     - manual
     - student
     - 1 month
     -
   * - courserestored
     - Course restored 2
     - 1
     - a summary
     -
     -
     -
     -
   * - courserestored
     - Course restored 3
     - 1
     - a summary
     -
     -
     -
     - padawan

