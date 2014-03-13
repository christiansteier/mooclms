.. _quiz:

Quiz
=====
The Quiz activity module allows the teacher to design and build quizzes consisting of a large variety of :ref:`Question types <question_types>` , including multiple choice, true-false, and short answer questions. These questions are kept in the :ref:`Question bank <question_bank>` and can be re-used in different quizzes. 

Features of quiz
------------------
  * Quizzes can be configured to allow multiple attempts. Each attempt at a question is automatically marked, and the teacher can choose whether to give feedback and/or show the correct answers. 

There are many ways to use a quiz.

  * Feedback about performance and self-assessment are important parts of a learning environment. There are several ways to give feedback to students: on each question or overall. The quiz module can display feedback and scores at different times during the quiz, using the review options in the Quiz settings. 
  * A wide variety of Quiz reports (in addition to Grades) are available for use by the teacher. Quiz reports not only can focus on a single student's attempt to answer each question, but also can perform a robust item analysis of a question's validity based upon aggregated student responses. 
  * A single quiz can automatically select random and/or specific questions from different categories of questions. 
  * There are different options for scoring (marks-grades) individual questions in a specific quiz, grading attempts for a quiz and each question type. 
  * The quiz settings allow different display methods. They can randomize the questions for each student and or randomize the answers for each student. 
  * The teacher can determine the number of questions on each page of questions the student sees. The teacher can change the position of any question in the quiz. It is possible to put a label with information any place between questions. 
  * The teacher can choose how questions behave during the quiz. It can be like a classic test, where the student gets no feedback while attempting the test, only later. Alternatively, Moodle can reveal the grades and/or feedback to the student during the quiz, and perhaps even give them another chance to answer the question (for fewer marks) having read the feedback. 

Creating a new quiz is a two-step process. In the first step, you create the quiz activity and set its options which specify the rules for interacting with the quiz. In the second step you add questions to the quiz. This page describes the options you can set for the quiz activity. The page Building Quiz describes how to set up the questions for the quiz.


Quiz administration
--------------------
When you first set up your quiz from *Add an activity or resource > Quiz*, (or, if you don't have this link, the dropdown *Add an activity > Quiz*) you will get the following settings, (which can also be changed later in the Edit Settings link of the Quiz administration settings block) All settings may expanded by clicking the "Expand all" link top right. 

General
^^^^^^^^

**Name**
    
This is the standard name field. This name will appear on the home page of the course, navigation menu and other places which will show or provide links to this quiz. 

**Description**

Describe the purpose of the glossary and provide instructions or background information, links etc. Click the icon top left to expand the toolbars, and drag the bottom right of the text box out to expand it. 

**Display description on course page**
    
If ticked, the quiz description will appear on the course page directly under the quiz name. 

Timing
^^^^^^^
(These settings are collapsed by default) 

**Open the quiz**

You can specify times when the quiz is accessible for people to make attempts. Before the opening time the quiz will be unavailable to students. They will be able to view the quiz introduction but will not be able to view the questions. Quizzes with start times in the future diasplay both the open and close date for students. 

**Note:** You can make the quiz available at different times for different groups or users in the Group or User override sections of the Quiz Administration settings block.

**Close the quiz**

After the closing time, the students will not be able to start new attempts. Answers that the student submits after the quiz closing date will be saved but they will not be marked. 

Even after the quiz has closed students will still be able to see the quiz description and review their attempts. What exactly they will see depends on the settings you choose for review options (see below). 

**Time limit**

By default, quizzes do not have a time limit, which allows students as much time as they need to complete the quiz. If you do specify a time limit, several things are done to try and ensure that quizzes are completed within that time.

  1. A countdown timer is shown in the quiz navigation block
  2. When the timer has run out, the quiz is submitted automatically with whatever answers have been filled in so far
  3. If a student manages to cheat and goes over the allotted time, no marks are awarded for any answers entered after the time ran out 

**Note:** You can make the quiz available last a different period of time for different groups or users in the Group or User override sections of the Quiz Administration settings block

**When time expires**

There are three options as to what will happen when the time limit is up. Choose the one you need from the dropdown menu:

**Submission grace period**

If you select "there is a grace period..." then you can check the box to enable the "Submission grace period" and specify a period of time during which learners may still submit the quiz after the time is up. 

Examples of how timing is handled
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  1. A student starts a quiz at noon. The quiz has a one-hour time-limit, and a 1 hour delay between attempts. The student gets distracted, and so actually does not submit (using the overdue handling) until 1:30pm. *They are allowed to start their second attempt at 2. pm*
  2. The quiz count-down timer submits a student's quiz attempt at the last second when time expires. Because the server is heavily loaded, it takes 30 seconds to process the student's attempt. *The submission is accepted nonetheless*.
  3. Same situation as above but with a 120 second delay: *The submission is rejected*.
  4. The delay is not because of server load but because the student found a way to cheat the timer. *Moodle cannot know what causes a delay.The behaviour is controlled by the admin setting(quiz | graceperiodmin), 60 seconds by default*.
  5. A student is a member of 3 groups,all of which have different override settings. Which limits will apply to this student? *If there is any user-specific override, then that is used, and the group overrides for that setting are not used at all. Otherwise, if there are multiple group overrides, the most generous values are used (the earliest open date, the latest close date, the longest time limit, the most number of attempts, and the student can type any of the passwords)*.
  
Grade
^^^^^^
(These settings are collapsed by default) 

**Grade category**

If you have categories in your gradebook, select the one you wish the quiz to be in here.

**Attempts allowed**

Students may be allowed to have multiple attempts at a quiz. This can help make the process of taking the quiz more of an educational activity rather than simply an assessment. If the quiz is randomized then the student will get a new version for each attempt. This is useful for practice purposes. 

**Note:** You can change the allowed number of attempts for different groups or users in the Group or User override sections of the Quiz Administration settings block.

**Grading method**

When multiple attempts are allowed, there are different ways you can use the grades to calculate the student's final grade for the quiz. 

  * Highest grade - the final grade is the highest (best) grade in any attempt
  * Average grade - the final grade is the average (simple mean) grade of all attempts
  * First grade - the final grade is the grade earned on the first attempt (other attempts are ignored)
  * Last grade - the final grade is the grade earned on the most recent attempt only 

Layout
^^^^^^^
(These settings are collapsed by default) 

**Question order**

If 'Shuffled randomly' is selected, then the order of questions in the quiz will be randomly shuffled each time a student starts a new attempt at the quiz. The intention is to make it a little harder for students to copy from each other. 

**New page**

For longer quizzes it makes sense to stretch the quiz over several pages by limiting the number of questions per page. When adding questions to the quiz, page breaks will automatically be inserted according to the setting you choose here. However, you will also be able to move page breaks around by hand later on the editing page. **Note that changing this setting has no effect on questions you have already added to the quiz**. The setting will only apply to questions you add subsequently. To change the page breaks in an existing quiz, you need to go to the quiz editing screen, tick the 'Show page breaks' checkbox, then use the repaginate control. 

**Navigation method** (available by clicking Show More)

By choosing Sequential instead of Free, the teacher is forcing the student to progress through the questions in order without being able to go back to a previous question or skip to a later one. 

Question behaviour
^^^^^^^^^^^^^^^^^^^
(These settings are collapsed by default) 

**Shuffle within questions**

If set to 'yes', then each time the student takes a quiz the parts of the question will be shuffled randomly.

**How questions behave**

  * **Deferred feedback** - Students must enter an answer to each question and then submit the entire quiz, before anything is graded or they get any feedback.
  * **Adaptive mode and Adaptive mode (no penalties)** - Allows students to have multiple attempts at the question before moving on to the next question.
  * **Interactive mode** - After submitting one answer, and reading the feedback, the student has to click a 'Try again' button before they can try a new response. Once the student has got the question right, they can no longer change their response. Once the student has got the question wrong too many times, they are just graded wrong (or partially correct) and get shown the feedback and can no longer change their answer.
      * There can be different feedback after each try the student makes.
      * The question can adapt itself to the student's answer, for example by giving some hints before asking the student to try again. 
  * **Immediate feedback** - Similar to interactive mode in that the student can submit their response immediately during the quiz attempt, and get it graded. However, they can only submit one response, they cannot change it later.
  * **Deferred feedback or Immediate feedback with Certainty-based marking (CBM)** - With CBM, the student does not only answer the question, but they also indicate how sure they are they got the question right. The grading is adjusted by the choice of certainty, so that students have to reflect honestly on their own level of knowledge in order to get the best mark. See the See Also section below for an example quiz using CBM and a blog post explaining the philosophy. 

**Note:** There is also an option "Manual grading" which can be enabled from Administration>Site administration>Plugins>Question behaviour This causes all questions in the quiz to require manual grading. 



















