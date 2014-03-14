.. _numerical_question_type:

Numerical question type
========================
From the student perspective, a numerical question looks just like a short-answer question. The difference is that numerical answers are allowed to have an accepted error. This allows a fixed range of answers to be evaluated as one answer.

For example, if the answer is 30 with an accepted error of 5, then any number between 25 and 35 will be accepted as correct.

You are able to

  * grade independently the number and the unit,
  * choose to handle the unit response either as
  
      * a text input element or as
      * a multichoice radio element, 
  * just grade the number with the option to write the unit close to the input element,
  * put the unit either
  
      * at right of the number as the most common occurence
      * or at left as in $ 100,00. 

Furthermore your valid number formats and specific intructions on how to answer will be put near the answer input element. An example 

Questions may have different answers with different levels of accuracy. That lets you create questions like "What is a root of x^2 - 3x + 2?" and award different levels of credit depending on the accuracy of the answer.

Text answers are no longer allowed - Short-Answer question type should be used instead.


Numerical question set-up
---------------------------
  1. In Quiz or Question bank
  2. Select the question category
  3. Give the question a descriptive name - this allows you to identify it in the question bank.
  4. Enter a question in the 'question text' field. This can include an equation - Moodle has a couple of text filters that allow you to type an equation and have it properly typeset when displayed. The Algebra filter is very good for writing common mathematical expressions in a simple way. More complicated expressions may be written using the TeX filter. Filters contains information for administrators on how to enable these filters. Alternatively, select an image to display if you want to add a picture to the question.
  5. Select an image to display if you want to add a picture to the question. For the student, it appears immediately after the question text and before the choices.
  6. Set the 'default question grade' (i.e. the maximum number of marks for this question).
  7. Set the 'Penalty factor' (see Penalty factor below).
  8. Add general feedback. This is text that appears to the student after he/she has answered the question.
  9. Now enter the first accepted answer(s). Note: Floating point numbers, e.g. 23.4, may also be written as 23,4 or 2.34E+1.
  10. Enter an accepted error for this answer. This is the range above or below the answer that Moodle will accept as a match. For example, if the correct answer is 5, but you will accept 4 or 6 as answers, your accepted error is 1.
  11. Enter a grade for this answer.
  12. Enter feedback for the accepted answer. This is the text that the student will see if they enter a number within the accepted error of the answer.
  13. Repeat for each of the answers you want to accept. You can provide feedback for all wrong answers by using a wildcard, i.e. the asterisk character (*), as an answer with grade 'None'.
  14. Units can also be specified. For example, if you enter a unit of 'cm' here, and the accepted answer is 15, then the answers '15cm' and '15' are both accepted as correct. You can also specify a multiplier. So, if your main answer was 5500 with unit W, you can also add the unit kW with a multiplier of 0.001. This means that the answers '5500', '5500W' or '5.5kW' would all be marked correct. Note that the accepted error is also multiplied, so an allowed error of 100W would become an error of 0.1kW.
  15. Click 'Save changes' to add the question to the category. 

Penalty factor
^^^^^^^^^^^^^^^
The 'penalty factor' only applies when the question is used in a quiz using adaptive mode - i.e. where the student is allowed multiple attempts at a question even within the same attempt at the quiz. If the penalty factor is more than 0, then the student will lose that proportion of the maximum grade upon each successive attempt. For example, if the default question grade is 10, and the penalty factor is 0.2, then each successive attempt after the first one will incur a penalty of 0.2 x 10 = 2 points. 

Tips and tricks
-----------------
Remember that numerical questions in the Quiz module are slightly different than those in the Lesson module. 








