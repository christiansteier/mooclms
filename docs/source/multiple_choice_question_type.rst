.. _multiple_choice_question_type:

Multiple Choice question type
==============================
Moodle provides teachers with a lot of flexibility when creating this common question type. You can create single-answer and multiple-answer questions, include pictures, sound or other media in the question and/or answer options (by inserting HTML) and weight individual answers. Remember that Lesson module questions behave differently.

There are two types of multiple choice questions - single answer and multiple answer. 

Single-answer questions
^^^^^^^^^^^^^^^^^^^^^^^^
These questions allow one and only one answer to be chosen by providing radio buttons next to the answers. You will specify non-negative marks for each answer, usually zero marks for wrong answers, maximum marks for correct answers and partial marks for partially correct answers. 

Multiple-answer questions
^^^^^^^^^^^^^^^^^^^^^^^^^^
The teacher can select "multiple answers are allowed" in a Multiple Choice question type. "Multiple answers" questions types in a quiz allow one or more answers to be chosen by providing check boxes next to the answers. Each answer may carry a positive or negative grade, so that choosing ALL the options will not necessarily result in good grade. If the total grade is negative then the total grade for this question will be zero.

Feedback can be associated either with specific answers, or with the question as a whole. 

Question set-up
----------------
  1. Select the question category
  2. Give the question a descriptive name. You'll use the name to track your questions later so "Question 1" isn't a good idea. The name will be used in the question lists on the quiz editing page or in the lesson as a page title. It will not be shown to the students, so you can choose any name that makes sense to you and possibly other teachers.
  3. Create the question text. If you're using the HTML Editor, you can format the question just like a word processing document.
  4. Select an image to display if you want to add a picture to the question. The available images are those you have uploaded to the main Moodle files area (they cannot be in folders). For the student, the image appears immediately after the question text and before the answer options.
        * Alternatively, if you used the HTML editor to create the question text, you can click the image icon. This will pop up the Insert Image window. You can choose to upload an image into your files area from this window, or you can add the URL of an image on the web. If you add a file to your files area, click the name of the file after you upload it to insert the link into the URL text entry at the top of the screen. Then click OK. 
  5. Set the 'default question grade' (i.e. the maximum number of marks for this question).
  6. Set the 'Penalty factor' (see Penalty factor below).
  7. Moodle 1.7+: If you wish, add general feedback. This is text that appears to the student after he/she has answered the question.
  8. Choose whether students can only select one answer or multiple answers
  9. Choose whether to shuffle the answer options
  10. Write your first answer in the Choice 1 text field. Inserting HTML into this area also makes it possible to add an image or a sound file.
  11. Select a grade percentage for the answer. This is the percentage of the total points for the question that selecting this response is worth. You can select negative percentages as well as positive percentages. So, selecting a correct response in a multiple answer question may give you 50% of the possible points, while selecting a wrong answer may take away 10%. Note that in a multiple-answer question, the grades must add up to 100%.
  12. If you wish, you can add feedback for each response. It may be a bit more work, but it’s good practice to tell the students why each answer is right or wrong using the feedback area. If students know why an answer is right or wrong, they can analyse their own thinking and begin to understand why an answer is correct. Your feedback will only be displayed if you select Show Feedback in the quiz body options.
  13. Fill in the rest of the response choices in the rest of the form. Any unused areas will be ignored.
  14. Moodle 1.7+: Fill in the overall feedback fields if you wish.
  15. Select the "Save Changes" button at the bottom of the screen. 
  
Penalty factor
^^^^^^^^^^^^^^^^
The 'penalty factor' only applies when the question is used in a quiz using adaptive mode - i.e. where the student is allowed multiple attempts at a question even within the same attempt at the quiz. If the penalty factor is more than 0, then the student will lose that proportion of the maximum grade upon each successive attempt. For example, if the default question grade is 10, and the penalty factor is 0.2, then each successive attempt after the first one will incur a penalty of 0.2 x 10 = 2 points. 

General feedback
-----------------
General feedback is some text that gets shown to the student after they have attempted the question. Unlike feedback, which depends on the question type and what response the student gave, the same general feedback text is shown to all students.

You can control when general feedback is shown to students using the "Students may review:" check-boxes on the quiz editing form.

You can use the general feedback to give students some background to what knowledge the question was testing. Or to give them a link to more information they can use if they did not understand the questions. 

Overall feedback
-----------------










