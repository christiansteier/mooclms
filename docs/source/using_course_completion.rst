.. _using_course_completion:

Using course completion
========================
Course completion can be used in many ways. It is important to remember that this feature is only a reporting feature.

While course completion will not lock a student out of another course, it will allow a teacher to see if a student has completed the recommended prerequisite courses.

It can also work with Activity completion to show students the activities they have completed. This can be via a check mark next to the activity on the course's home page, or by looking at the :ref:`Course completion status block <course_completion_status_block>`.

It is a way to ensure that the teaching team's members sign off that a student has completed the course. For example, Teacher B is the instructor for Course2, which has a recommended prerequisite for completing Course1. Teacher B, is the non-editing teacher in Course1 and must check the box that indicates the student has completed the course. 

In the above Example, the teacher has not checked off that "Test User1" has finished this course. 

Courses can be linked via their course completion criterion.

**Note:** The course completion feature works with Cron. Thus changes in reports may not appear until after cron.php has run.

Manual completions
--------------------
Depending upon the settings, course completion can require that an activity or the entire course be manually marked as complete. The settings will allow any number of combinations. For example, an activity might require the student to receive a minimum score and have the non-editing teacher manually check complete. Or merely require the student to check an activity or the course as complete. 

**Manual marking by student examples**

A course completion setting may require the student to confirm they have completed the course. Students do this by using the :ref:`Self completion block <self_completion_block>`.

A course completion setting may require a student to manually mark an activity when they believe they have finished it. On the course homepage, the student may see a box to check as a self completion of the activity.

**Manual marking by teacher examples**

In order for a teacher (or non editing teacher, Manager or other role) to mark a course as complete, the appropriate box in the Manual Completion by.. section must be checked in the completion tracking settings.

The teacher then accesses the :ref:`Course completion status block <course_completion_status_block>` and checks the names of the students who are deemed to have completed the course. 

Course completion based on specified criteria
----------------------------------------------
It is possible to have a course marked as complete dependent on a combination of specified criteria such as activities completed, grade achieved or length of time spent in the course. This is decided in the *overall criteria type aggregation*.

The settings for automatic course completion are described in more detail in Course completion settings and these include:

  * activities completed
  * date
  * duration after enrolment
  * grade
  * unenrolment 

    See Example 1, Example 2 and Example 4. 

Course completion report
--------------------------
Course completion info can be viewed by managers, teachers and non-editing teachers (and any other users with the capability report/completion:view) in *Administration> Course administration > Course completion* or via a link in the Course completion status block. 

