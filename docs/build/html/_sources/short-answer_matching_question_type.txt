.. _short-answer_matching_question_type:

Random Short-answer Matching question type
===========================================
Note: The Random Short-Answer Matching question type is broken in Moodle versions 2.6 and 2.6.1, and can be used again starting from Moodle 2.6.2.

  * From the student perspective, this looks just like a Matching question. The difference is that the sub-questions are drawn randomly from the Short Answer questions in the current category (including or not subcategories from the current category).
  * After an optional introduction, the respondent is presented with two or more sub-questions, each with a drop-down menu box opposite listing the same number (or fewer if several sub-questions have the same answer) of available answer options.
  * The respondent must select an answer option to match each sub-question.
  * Each sub-question is equally weighted to contribute towards the grade for the total question.
  * The questions and answers are randomly drawn from the pool of short-answer questions in the current category (and in its subcategories if this option was selected).
  * You must make sure that the category contains enough short-answer questions, otherwise the student will get an error message. The more short-answer questions you add to the category, the more likely it is that students will see a new selection on each attempt. Short answers questions used in a previous attempt to the same question or in another Random Short-Answer question of the same quiz are not excluded, so you should ensure there are enough Short Answer questions in the category to mitigate the risk of a student getting the same questions and answers.
  * Note that the answer options are taken from the correct (having a 100% grade) answers of each contributing short-answer question. If there are several answers to the sort-answer question with a 100% grade, the first one is used. Therefore, if the short-answer questions in this category are on different topics, this question type will not be useful, as the correct option will be obvious. 


An example that doesn't work - suppose the category contains 2 short-answer questions, as follows:

+---------------------------------------------------------------+
| 1. What is the capital of France?                             |
|  Correct answer: Paris                                        |
|  Other recognised answers: Lyon, Marseilles, *                |
| 2. What vegetable is called 'løk' in Norway?                  |
|  Correct answer: Onion                                        |
|  Other recognised answers: Leek, *                            |
+---------------------------------------------------------------+

   The result will appear as follows:
   
+---------------------------------------------------------------+
| What is the capital of France?                                |
|  - Options: Paris, Onion.                                     |
| What vegetable is called 'løk' in Norway?                     |
|  - Options: Paris, Onion.                                     | 
+---------------------------------------------------------------+


An example that does work - suppose the category contains 2 short-answer questions, as follows:

+---------------------------------------------------------------+
| 1. What is the capital of France?                             |
|  Correct answer: Paris                                        |
|  Other recognised answers: Lyon, Marseilles, *                |
| 2. In what city is Le Corbusier's "Unite d'Habitation"?       |
|  Correct answer: Marseilles                                   |
|  Other recognised answers: Paris, Lyon *                      |
+---------------------------------------------------------------+

   The result will appear as follows:
   
+---------------------------------------------------------------+
| What is the capital of France?                                |
|  - Options: Paris, Marseilles.                                |
| In what city is Le Corbusier's "Unite d'Habitation"?          |
|  - Options: Paris, Marseilles.                                | 
+---------------------------------------------------------------+


Question set-up
----------------
  1. Select the question category.
  2. Give the question a descriptive name - this allows you to identify it in the question bank.
  3. Enter the question text to tell the students what they are matching. 
  4. Set the 'default question grade' (i.e. the maximum number of marks for this question).
  5. Set the 'Penalty factor' (see Penalty factor below).
  6. If you wish, add general feedback. This is text that appears to the student after he/she has answered the question.
  7. Select the number of questions you want to add to the matching question - make sure this is less than or equal to the number of short-answer questions available in this category (a verification will be done when the question is saved).
  8. Select if you want questions to be drawn also from subcategories of the current category
  9. Click Save changes. 

Penalty factor
^^^^^^^^^^^^^^^
The 'penalty factor' only applies when the question is used in a quiz using adaptive behaviour - i.e. where the student is allowed multiple attempts at a question even within the same attempt at the quiz. If the penalty factor is more than 0, then the student will lose that proportion of the maximum grade upon each successive attempt. For example, if the default question grade is 10, and the penalty factor is 0.2, then each successive attempt after the first one will incur a penalty of 0.2 x 10 = 2 points. 













