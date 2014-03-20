.. _building_quiz:

Building Quiz
==============

How a Moodle quiz works?
-------------------------
The word “quiz” might conjure up for some images of TV game shows, but a Moodle quiz is basically a set of questions presented to the learner which may be automatically marked by Moodle or graded later by the teacher. The questions may be in sentence or number form or contain various media such as video or sound. They do not all need to be the same type of questions: a quiz may contain multiple choice, matching, essays (teacher-graded) and calculated. Feedback may be given at any or all stages of the process.

If a quiz is a book, the Quiz settings are equivalent to the front cover; the quiz itself is contained within when the questions are created. (Be careful : once you have chosen the Quiz Settings, it will be “live” on your course page, unless you hide it, so your learners could potentially see a quiz with no questions, like a front cover with no content.)

Once a quiz has been added to the course and the Quiz settings established,the teacher can start to build the quiz. The teacher can access the quiz to edit the questions by clicking directly on the Quiz name on the course home page and then "Edit quiz" or by clicking the "info" link in the Navigation block. The "Edit quiz link can also be accessed from *Administration > Quiz administration*. 

Adding questions
------------------
Once you have accessed the quiz editing screen as above, you can add questions from a number of locations:

  1. Click the "Add question" button to begin a new question (1 below)
  2. Click "Show" (2a) to reveal the contents of the question bank (2b) and then choose a pre-made question or click "Create new question" (3)
  3. Click "Add a random question" to add a random question, *providing there are questions in the question bank already*.
  
Creating a new question
^^^^^^^^^^^^^^^^^^^^^^^^^
  1. To make a brand new question, click "Add a question".
  2. From the next screen, choose the question type you want to add and click "Next"

**NOTE:** When you click on a question type on the left, helpful information appears on the right. 

  3. Fill in the question form, making sure to give a grade to the correct answer.
  4. Click "Save changes" 
  
**Adding responses and feedback**
When you add responses and feedback you can display one or more toolbars in the editor.
Note that when a question has been created, an icon and words display its type (eg multiple choice) and a magnifiying glass icon allows you to preview it.
You can continue adding questions this way, clicking the "Add a question" button each time. 

Choosing a pre-made question
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
If other teachers in the course have made questions, or if a teacher made questions in an earlier quiz, these can be added to the current quiz by clicking the arrows next to them in the question bank (1 below) or by checking/ticking the box of several and then clicking the button "add to quiz" (2). To ensure all previously made questions are available, make sure to tick the boxes "also show questions from sub-categories/old questions". 

Adding a random question
^^^^^^^^^^^^^^^^^^^^^^^^^
As long as you have questions in the question bank, you can add random questions to your quiz (3 above). This might be useful if you have students in a class taking a quiz at the same time, because they are unlikely to get the same questions at the same time. The same question will never appear twice in a quiz. If you include several random questions then different questions will always be chosen for each of them. If you mix random questions with non-random questions then the random questions will be chosen so that they do not duplicate one of the non-random questions. This does imply that you need to provide enough questions in the category from which the random questions are chosen, otherwise the student will be shown a friendly error message. The more questions you provide the more likely it will be that students get different questions on each attempt.

The grade for the randomly chosen question will be rescaled so that the maximum grade is what you have chosen as the grade for the random question.

You can add one or more random questions by choosing the number and category in the question bank. Note the die icon to highlight random question selection. 

Question categories
^^^^^^^^^^^^^^^^^^^^
Questions can be stored and retrieved from categories in the Question bank. When you make a new question it defaults to the category with the course name. So if you make a quiz in the Senior Physics course, questions will automatically be added to "Default for Senior Physics". You can opt to have your quiz questions in a category of their own ("Quizname") or to add a subcategory.

To add a subcategory, go to *Administration > Quiz administration > Question bank > Categories* For more information on question contexts and categories, see :ref:`Question bank <question_bank>`.

Users will have access to different categories according to their permissions. For example, a regular teacher might only have access to question categories in his own Physics course whereas his Faculty Head of Science with permissions in all science courses might have access to question categories in Biology and Chemistry as well. 

Quiz layout
------------
  * You can choose in Administration>Quiz administration>Edit settings>Layout whether to have a new page for every question or after a certain number of questions.
  * You can click the "Add a page here" button to add a page at selected intervals and move questions up and down by clicking the arrow button.
  * You can also set the pages by clicking the tab "Order and paging" on the Edit quiz screen.
  * Questions may be moved up and down with the arrows, or you can check the boxes to their left and then click "reorder questions"
  * You can check a box to select a question and then click "Add new pages after selected questions"
  * You can "repaginate" by setting the number of questions per page. After setting the number of questions per page, you can move questions so that there are a different number of questions on each page. 

Assigning points to questions
-------------------------------
*Administration > Quiz administration > Edit quiz > Editing quiz*

You can set how many points each question is worth by changing the number in the box to the right of each question (1) and you can change the maximum grade by changing the number in the box at the top of the quiz (2) The default is one point per question and 100.00 maximum grade. 

**Tip:** Each save button is independent of each other. Thus if you change 2 grade boxes and click on the "Save" button, only the grade next to that button will be saved. Your other changes will revert to what they were before. Best practice is to change the grade and save one question at a time. 

The quiz module will do any maths, so for example, a 2 point question will be worth 2 times more when the Quiz module determines how many point out of 10 to award the student. 

Previewing the quiz
---------------------
  * You can preview individual questions by clicking the magnifying glass icon.
  * You can preview the whole quiz by clicking the "Preview" link in *Administration > Quiz administration > Preview*
  * The quiz works like a real quiz so you can see your grades and any feedback for correct/incorrect answers just as a student would see them. 

After quiz has been attempted
-------------------------------
If one or more students have taken the quiz, you will see a list of all the questions in the quiz and a notice saying that you cannot add or remove questions.

You can change the order of questions, regrade them, preview an individual question and click on an question edit link that will allow you to directly edit the question stored in the question bank.

**NOTE:** You can delete all quiz attempts by students and then edit the quiz as if no students had attempted it. To do this,click the quiz name and then the Results link in the Navigation block. This will present a list of students and their scores. Click "Select all" and then "Delete selected attempts".

Dealing with faulty questions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
There are several ways to deal with "bad" questions in a quiz.

  * Change the grade for the bad question to 0 in the quiz.
  * Edit the question, changing what you will accept as a correct answer, then regrading the exam. Remember when changing a question that the next time it is used it will be as it was in the last edit. Also, regrading will only affect one quiz at a time.
  * You can edit the question to explain the situation to the student and then you can set the grade for the question to zero. After you make such changes you should regrade the quiz by clicking on the *Results* tab and then the *Regrade* tab. This will change the grade for all students who have taken the quiz so far. Remember, if the question is used by another quiz, your "explanation" will appear as part of that quiz.
  * You can change the grade for the bad question and then move or delete the question from your question category. The question will still appear on the quiz. Some places do not like to delete any question, but will move them to a "dead" or "bad" question category.
  * When you discover a bad question in your quiz, it may affect the question bank. Remember that a final might be made up of a certain number of random questions drawn from different question categories, the same categories used in a smaller subject quiz. It can be very important do something about bad or invalid questions in a question category when the categories are use in other places. 












