.. _using_lesson:

Using Lesson
=============
This page outlines how students and teachers interact with Moodle lessons once they have been created. For details on how to set up and then organise a lesson, see :ref:`Lesson settings <lesson>` and :ref:`Building Lesson <building_lesson>`.

What the student sees
-----------------------
  * A student clicking on a Lesson will see an introductory page with one or more buttons which they choose from to select the path they wish to take.
  * The display may vary according to how the teacher has set up the lesson in Lesson settings. For example; there may or may not be a list of pages down the side; there may or may not be an ongoing score.
  * Students progress through the lesson with either content pages (of information, which is not graded) or various types of question pages(which may be graded) When a question page is used, the following page gives the answer and feedback if offered.
  * The lesson is ended when the student has met the criteria set by the teacher. This could be answering a certain number of questions correctly, accessing a certain number of pages with content (text, audio or video) or following a certain navigational path. A final page appears where the student can check their score, if applicable, and return to the main course page.   

What the teacher sees
-----------------------
A teacher clicking on a lesson will see tabs at the top offering them the chance to preview, edit, view reports or grade essays in the lesson.
    
**Preview** - The lesson opens up in preview mode for the teacher. However, it will not show the score unless the teacher switches their role to a student. 

**Edit** - The Edit tab allows teachers to alter the lesson once it has been set up. There are two views - Collapsed and Expanded. See :ref:`Building Lesson <building_lesson>` for more details on editing the lesson. 

**Reports** - The reports tab shows the performance of students taking the lesson. There is a general "Overview" and a "Detailed Statistics" tab. 

**Overview** - By clicking on the specific attempt, the teacher can view the student's answers to specific questions. It is also possible to delete a student attempt by checking the attempt and using the pull down menu to change "Choose" to "Delete". Below the "Overview" can also be seen general statistics: Average score, Average time, High score, Low score, High time, Low time. 

**Detailed statistics** - More detailed reports on individual questions are available from this tab.

**Grade essays** - Any essay questions which have been set in the lesson can be accessed and graded here. 


Grading lessons
-----------------
Note that for a lesson to be graded, it must have at least one question where a student can receive a score and the lesson can not be a practice lesson. Grades are calculated when the student has completed a lesson. Grades are kept for every student attempt. 
    
Understanding Flow control
----------------------------
1. *Administration > Lesson administration > Edit settings > Flow control group*
2. Here are some examples to help you understand the Lesson flow control settings. Please note:
3. "Allow student review" setting applies to the review of a whole Lesson, whereas
4. "Provide option to try a question again" setting applies to the review of an individual question page. When the student does not select the correct answer, 'Provide option to try a question again" setting will display 2 buttons. One will direct the student back to the question and the other to continue.
5. "Maximum number of attempts" is designed to prevent a student from being stuck on "This page" where they continually put or select the wrong answer. It will override other settings, such as review or the option to try the question again. When exceeded, it will not allow a score to be recorded for that question. 

Case 1
^^^^^^^
The teacher wants the student to be able to attempt any question no more than 3 times and be given the chance to answer the question again. The teacher wants the student to see the response attached to their answer.

Flow control settings

  * Allow student review **Yes** 
  * Provide option to try a question again **No** 
  * Maximum number of attempts **3** 
  * Display default feedback **No** 
  * Number of pages to show **0** 
  * Slideshow **No** 

Student selects wrong answer and will see:
  * "Response for the wrong answer" (if any is shown) 
  * "Yes, I'd like to try again" button 
  * "Continue" button. 

Student selects correct answer and will see:
  * "Response for the correct answer" (if any is shown) 
  * "Continue" button 

Case 2
^^^^^^^
The teacher wants to allow the student 3 attempts at all questions but not see any feedback except the site default feedback for wrong answers. 

Flow control settings 

  * Allow student review **No** 
  * Provide option to try a question again **Yes** 
  * Maximum number of attempts **3** 
  * Display default feedback **No** 
  * Number of pages to show **0** 
  * Slideshow **No** 

Student selects wrong answer and will see: 

  * Not quite. Would you like to try again? as text over the 
  * "Yes, I'd like to try again" button 
  * '"No, I just want to go on to the next question" button 

  **Note**: If the wrong answer jump is set to "This page" and the number of attempts is under the maximum, then the student will return to the question, regardless if they select "No, I just want to go on". 

Student selects correct answer and will see: 

  * "Your answer: {gives the student's answer)" 
  * Response attached to the correct answer (if any) 

Case 3
^^^^^^^
"Speed bump for speed clickers". Teacher only wants the student to get once chance to record an answer on any question. They will only see the response the teacher provides for any question, or the default feedback if no response has been set for the answer the student selected.

Flow control settings 

  * Allow student review **No** 
  * Provide option to try a question again **No** 
  * Maximum number of attempts **1** 
  * Display default feedback **Yes** 
  * Number of pages to show **0** 
  * Slideshow **No** 

Student selects wrong answer and will see: 

  * "Response for the wrong answer" (if any is shown) 
  * "Yes, I'd like to try again" button 
  * "Continue" button. 

  **Note:** When teacher sets the Jump to "This page" for a wrong answer, they will return to the page but their score will not change. 

Student 

  * "Response for the correct answer" (if any is show) 
  * "Continue" button 


