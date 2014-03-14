.. _short_answer_question_type:

Short Answer question type
===========================
In a short answer question, the student types in a word or phrase in response to a question (that may include a image). Answers may or may not be case sensitive. The answer could be a word or a phrase, but it must match one of your acceptable answers exactly. It's a good idea to keep the required answer as short as possible to avoid missing a correct answer that's phrased differently.

The Quiz and Lesson modules both have short answer question types. The analysis of the question given below works for both modules.

Question set-up
-----------------
  1. Select the question category
  2. Give your question a descriptive name.
  3. Create the question text. If you're using the HTML Editor, you can format the question just like a word processing document.
        **Tip:** if the answer is intended to fill a gap in the text, use underscores (5 or more) to indicate where the gap is. 
  4. Select an image to display if you want to add a picture to the question.
  5. Set the 'default question grade' (i.e. the maximum number of marks for this question).
  6. Set the 'Penalty factor' (see Penalty factor below).
  7. If you wish, add general feedback. This is text that appears to the student after he/she has answered the question.
  8. Choose whether the answers are case-sensitive. Case sensitivity can be tricky where capitalization is important. Will you accept Ban Ki-moon as well as ban ki-moon as an answer?
  9. Next, fill in the answers you will accept. You could give common misspellings partial credit with this option. For example will you accept "Ban Ki moon"? Use wildcards to allow for variants on a word pr phrase.
  10. Add grade for each answer.
  11. Create feedback for any and all answers. This will appear if the student enters that answer.
        Note: It is good practice to add a single wild card * for the last answer, so you can create a feedback response and a score for all other answers students might have. 
  12. Click Save Changes to add the question to the category. 

Penalty factor
^^^^^^^^^^^^^^^
The 'penalty factor' only applies when the question is used in a quiz using adaptive mode - i.e. where the student is allowed multiple attempts at a question even within the same attempt at the quiz. If the penalty factor is more than 0, then the student will lose that proportion of the maximum grade upon each successive attempt. For example, if the default question grade is 10, and the penalty factor is 0.2, then each successive attempt after the first one will incur a penalty of 0.2 x 10 = 2 points. 

Wildcard usage
----------------
You can use the asterisk character (*) as a wildcard to match any series of characters. For example, use ran*ing to match any word or phrase starting with ran and ending with ing. If you really do want to match an asterisk then use a backslash like this: \*

If you want one question with the two answers fuel and oxygen, you ought to be able to limit the number of variants by writing fuel*oxygen 100%. This would accept **"fuel oxygen", "fuel, oxygen", "fuel; oxygen", "fuel and oxygen", "fuel & oxygen" "fuel oxygen", "fuel und oxygen" "fuel&&oxygen"**. It would even accept **"fuel or oxygen", "fuel but not oxygen" "fuel|oxygen"** which might not be so good but you can never be completely safe!

Here are some answers and scores for a question "What does a rocket burn?".

  1. oxygen*fuel with a score 100%
  2. *fuel* with a score 50%
  3. *oxygen* with a score 50%
  4. *air* with a score 40%
  5. * with a score of 0%

The order of the answers is important. The answers are evaluated from 1st to last. When a match is found the process stops. If no match is found the question is scored wrong and the general response is used. It is a good practice to put a wild card as the last answer so the evaluation process knows what to do when nothing above it matches.

Without wildcards, the answers are compared exactly, so be careful with your spelling! 

Feedback for wrong answers
----------------------------
When you wish to have short answer type questions, you naturally have a limited number of variations that would be acceptable. So in case you wish to give a feedback in case of a wrong answer, you must spell out the right answers exactly and then use * as a final answer which will have grade as zero, and feedback will be the one for wrong answer.

Effectively, ANYTHING other than the specific answers mentioned by you will be treated as this option due to wildcard and will be deemed wrong; it'll give 0 marks and show the feedback for a wrong answer.

Here is an example:

What is a rabbit?


.. line-block::

answer1: animal
feedback: right
grade: 100%

.. line-block::    

answer2: mammal
feedback: right
grade: 100%

.. line-block::      

answer3: vertebrate
feedback: right
grade: 100%

.. line-block::

answer4: *
feedback: ouch! that was wrong
grade: none

Remember: you cannot do negative marking in this type and ANYTHING other than your right answer will be treated as option 4 due to the wildcard and given that feedback and zero marks. 



















