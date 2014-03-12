.. _lesson:

Lesson
=======
The lesson module presents a series of HTML pages to the student who is usually asked to make some sort of choice underneath the content area. The choice will send them to a specific page in the Lesson. In a Lesson page's simplest form, the student can select a continue button at the bottom of the page, which will send them to the next page in the Lesson.

There are 2 basic Lesson page types that the student will see: question pages and content pages. There are also several advanced navigational pages which can meet more specialized needs of the Teacher. The Lesson module was designed to be adaptive and to use a student's choices to create a self directed lesson.

The main difference between a Lesson and other activity modules available in Moodle comes from its adaptive ability. With this tool, each choice the students makes can show a different teacher response/comment and send the student to a different page in the lesson. Thus with planning, the Lesson module can customize the presentation of content and questions to each student with no further action required by the teacher. 

Lesson administration settings
--------------------------------
This page explains the settings involved when first creating a lesson. To add a lesson to your Moodle course page:

  1. With the editing turned on, in the section you wish to add your lesson, click the "Add an activity or resource" link (or, if not present, the "Add an activity" drop down menu) and choose Lesson All settings may expanded by clicking the "Expand all" link top right. 

General
^^^^^^^^

**Name**

Whatever you type here will form the link learners click on to view the lesson so it is helpful to give it a name that suggests its purpose.

Appearance
^^^^^^^^^^^

**File pop**

If you want to include a link to a file on the lesson page for students to refer to, upload it here.

**Progress bar**

Choose this to show a bar at the bottom of the page showing how far into the lesson the student has got.

**Display ongoing score**

Choose this to let students see their score as they work through the lesson.

**Display left menu**

Choose this if you want to show a list of the pages in the Lesson so a student can see what is coming up.

**Minimum grade to display menu**

Choose this if you want the student to go through the lesson once and get a grade before they can (on review) see and navigate through all the different pages.

**Slideshow**

Please note that slideshow mode currently does not work for Moodle 2.

**Maximum Number of Answers**

Here you can set the default number of answer boxes available when you add your question or content pages. For instance, if you are only going to use True/False, you would only need 2. You can change this at any time so it's not crucial.

**Use default feedback**

Choose this if you want to show a set phrase regardless of their answer. If you have set your own default feedback such as "well done; correct" or "never mind; better luck next time" etc it will appear. If you have not, then Moodle's default feedback will appear.

**Link to next activity**

Choose this to give students a link to another activity when they reach the end of the lesson. (Note: this can also be achieved using Conditional activities) 

Availability
^^^^^^^^^^^^^
(These settings are collapsed by default) 

**Available from/Deadline**

Here you can set a start and end date and time for your Lesson.

**Time limit**

This allows you to set a time limit on the lesson. Students will see a countdown counter as they work. The timer does not stop them doing the lesson when the time is up, but correct answers are no longer scored. 

**Password protected lesson**

  * Change to "Yes" and enter the password if you want students only to access it when they know the password. 

Prerequisite lesson
^^^^^^^^^^^^^^^^^^^^
(These setings are collapsed by default) 

**Dependent on**

This allows access to the lesson to be dependent on students' performance in another lesson in the same course. (Note: this can also be achieved with Conditional activities)

**Time spent**

Decide here how long you want the student to have spent in the chosen previous lesson

**Completed**

Check this box if you want the student to have completed a previous lesson (according to Activity completion settings)

**Grade better than**

Enter the grade from the previous lesson which you want the student to have exceeded before they can attempt the current lesson. 

Flow control
^^^^^^^^^^^^^
(These settings are collapsed by default) 

**Allow Student Review**

This puts a "Review Lesson" button on the last screen of the lesson to encourage the student to navigate through the lesson again from the start.  Be sure to check other settings to allow them to change their answers.

**Provide option to try a question again**

This displays a button after an incorrectly answered question so that the student can try again (but not get credit for it) 

**TIP:** Leave this off if you are using essay questions.  

**Maximum Number of Attempts**

Decide here how many times you want students to be able to attempt each question. When they reach the maximum, they will be taken automatically to the next page. 

**Action after a Correct Answer**

Choose here where you want a student to be sent to if they get a question right. See Using Lesson for more details on this setting. The options are:

  * the next part of the Lesson (default setting)
  * a random, unexpected page
  * a random page which they have not yet answered. 

**Number of pages to show**

You only need this if you have set "Action after a correct answer" to show an unseen or unanswered page. Otherwise, all pages will be seen 

Grade
^^^^^^
(These settings are collapsed by default.) 

Set a grade and grade category here.

**Practice lesson**

Use this if you don't need the lesson to be scored/graded but just need students to work through some pages. Set this to Yes to have the same ungraded type Lesson in earlier versions of Moodle.

**Custom Scoring**

Use this to give a particular number score (negative or positive) to each answer

**Re-takes allowed**

Choose this if you want your students to be able to do the lesson more than once.

**Handling of re-take**

If you allow your students to re-take the lesson, then decide here if the grade for all lesson attempts is the mean or the maximum.

Note that the Question Analysis always uses the answers from the first tries of the lesson. Re-takes by students are ignored. 

**Minimum Number of Questions**

Set here the minimum number of questions that will be used to calculate a student's score. Students will be told how many they have answered and how many more they need to answer.

  * If you are using Content pages, then set this to 0.
  * If you use this setting, then add some explanatory text at the start of the lesson so the student knows how many questions they must answer as a minimum. (They may answer more. 

Common module settings
^^^^^^^^^^^^^^^^^^^^^^^
(These settings are collapsed by default.)

See :ref:`Common module settings <common_module_settings>`

Restrict access/Activity completion
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
(These settings are collapsed by default)

These settings are visible if :ref:`Conditional activities <conditional_activities_settings>` and :ref:`Activity completion <activity_completion_settings>` have been enabled in the site and the course.














