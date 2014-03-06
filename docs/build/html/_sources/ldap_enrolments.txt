.. _ldap_enrolments:

LDAP enrolments
================
**Location:** LDAP edit settings link in *Administration > Site administration > Plugins > Enrolments > Manage enrol plugins*

How to set up LDAP enrollment
-------------------------------
This describes how to set up Lightweight Directory Access Protocol (LDAP) enrollment in Moodle (first written by Lars Jensen). LDAP enrolment works best in Moodle when used in conjunction with LDAP authentication, and we're going to assume that you have already set Moodle up for LDAP authentication.

Assumptions
^^^^^^^^^^^^
    1. You are running a recent version of Moodle.
    2. You are using LDAP authentication as your primary authentication method.
    3. Each user in has a uid attribute in the users LDAP record, that matches the ID number in the same users Moodle profile (this can easily be arranged with a mapping on the Moodle LDAP Authentication setup page - for Active Directory, use 'distinguishedName', without the quotes) 
    
The Course Setup
^^^^^^^^^^^^^^^^^^
Our setup involves the following course and user definitions:

    * Two courses, Math101 and Eng201.
    * Two teachers, TeacherA and TeacherB.
    * Three students, StudentD, StudentE, and StudentF.
    * StudentD and StudentE are enrolled as students in Math101, and TeacherA is enrolled as teacher of Math101. StudentE and StudentF are enrolled as students in Eng201, and TeacherA and TeacherB are both enrolled as teachers of Eng201. 

The LDAP Container Setup
^^^^^^^^^^^^^^^^^^^^^^^^^^
    1. Define two LDAP containers ou=StudentEnrollment and ou=TeacherEnrollment
    2. For each course we define an LDAP group entry (e.g a posixGroup entry) in the StudentEnrollment and TeacherEnrollment containers. Thus, we define a Math101 posixGroup under StudentEnrollment, and we define a Math101 posixGroup under TeacherEnrollment. We define the two Eng201 groups in a similar way. Be careful, the name of the posixGroup has to match the Course ID number of the Moodle course. Do not use the course short name, it will not work.
    3. Enroll students and teachers as members of in the LDAP-groups we just defined. This is done by entering the users uid attribute (idnumber) in the memberUid attribute of the relevant group:
        * TeacherA is a member of the Math101 group under TeacherEnrollment.
        * StudentD and StudentE are a members of the Math101 group under StudentEnrollment.
        * TeacherA and TeacherB are members of the Eng201 group under TeacherEnrollment
        * StudentE and StudentF are a members of the Eng201 group under StudentEnrollment. 
        


