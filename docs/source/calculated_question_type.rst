.. _calculated_question_type:

Calculated question type
=========================
Calculated questions offer a way to create individual numerical questions by the use of wildcards (i.e you can use common variables names as **x , y** enclosed in curly braces to create the wildcards **{x}** and **{y}**) that are substituted with random values when the quiz is taken.

For example, if you want to create a large number of **"Calculate the area of a rectangle"** problems to drill your students, you could create a question with two wildcards (i.e. **{base}, {height}** created from the common **base, height** variable names) and put in the **"Correct Answer Formula="** input field **{base} * {height}** ( * being the multiplication sign ). 

+-------------------------------------------------------+
| **Correct Answer Formula=** {base}*{height}           |
+-------------------------------------------------------+

When a student takes the test, Moodle will randomly select values for **{base}** and **{height}** and grade the response using the result of the **Correct Answer Formula**.

The test will very rarely appear the same way twice. 

The main purpose of the calculated question is to create multiple versions of a question with different numerical values. This means you must have at least one wildcard in one of the answers.

If you don't need a random element, use the Numerical question type instead. 


Wildcards and datasets
------------------------
When Moodle delivers a Calculated question to the student, the wildcards are replaced with randomly-selected values. However, these values are not completely random - rather, they are randomly selected from a pre-defined *dataset* of possible values. This allows you some control over the possible values chosen - for example, in order to make sure the numbers are realistic.

These datasets can be *private or shared* - private datasets are used by one wildcard within one calculated question; shared datasets are used by one wildcard within all calculated questions that use it. 

Question set-up
----------------
To create (or modify) a calculated question there are three pages to work through. The instructions below take you through the pages, step by step: 

Page 1. Editing a Calculated question
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  1. Select the question **category**
  2. Any shared wildcards for this category are listed beneath. If you change category, you'll need to click the "Update the category" button to refresh this list. There may not be any shared wildcards yet - if not, you can create them later if you wish.
  3. Give the question a descriptive **name** - this allows you to identify it in the question bank.
  4. Enter the **question text**. This should be the question you want the student to answer, and it must include all the information they need to calculate an answer. Therefore it must contain at least one wildcard, inside curly braces. For example, if you wanted the student to sum numbers A and B, the question text might read: "What is {A} + {B}?" You may also include quantities computed from wildcards using the syntax "{=...}: for example, the question "What is {={A}+{B}} - {A}?" with wildcard values A=4 and B=3 would display as "What is 7 - 4?"
  5. Select an image to display if you want to add a picture to the question. For the student, it appears immediately after the question text and before the choices. If you want more control over how the image appears, include it in the question text above, using the HTML editor.
  6. Set the **default question grade** (i.e. the maximum number of marks for this question).
  7. Set the **Penalty factor** (see Penalty factor below). 
  8. Moodle 1.7+: If you wish, add general feedback. This is text that appears to the student after he/she has answered the question.
  9. Next add the **formula for the answer**. This formula must contain at least the wildcards that appear in the question text. See Correct answer formula syntax below.
  10. Choose the **grade** that the student will get for this question if they give this answer. This should be a percentage of the total marks available. For example, you could give 100% for a correct answer, and 50% for an answer that is nearly right. **One of the answers must have a 100% grade**.
  11. Determine the **tolerance** for error that you will accept in the answer. The tolerance and tolerance type settings combine to give a range of acceptable scores. So, if tolerance = t, correct answer = x and the difference between the user's answer and the correct answer is dx, then the tolerance types are as follows:

       * Nominal - mark correct if dx <= t
       * Relative - mark correct if dx / x <= t
       * Geometric - mark correct if dx² / x² <= t² 

  12. The next 2 settings, "Correct answer shows" and "Format" determine the **precision** of the answer. Use these to select the number of decimal places or significant figures you want to use.
  13. Add some **feedback** which the student will see if they enter this answer.
  14. You can specify as many answer formulae as you like - click "Add another answer blank" to add more.
  15. You can also specify units for the answers. For example, if you enter a unit of 'cm' here, and the accepted answer is 15, then the answers '15cm' and '15' are both accepted as correct. If you add more than one unit, you can also specify a multiplier. So, if your main answer was 5500 with unit W, you can also add the unit kW with a multiplier of 0.001. This means that the answers '5500', '5500W' or '5.5kW' would all be marked correct. Note that the accepted error is also multiplied, so an allowed error of 100W would become an error of 0.1kW.
  16. Finally (!) you can click "Next page" to save what you've done and move on. If you are editing an existing question, you can click "Next page (new question)" to create a completely new question based on an existing one. 

**Penalty factor**

The 'penalty factor' only applies when the question is used in a quiz using adaptive mode - i.e. where the student is allowed multiple attempts at a question even within the same attempt at the quiz. If the penalty factor is more than 0, then the student will lose that proportion of the maximum grade upon each successive attempt. For example, if the default question grade is 10, and the penalty factor is 0.2, then each successive attempt after the first one will incur a penalty of 0.2 x 10 = 2 points. 

**Tolerance**

As for numerical questions it is possible to allow a margin within which all responses are accepted as correct. The "Tolerance" field is used for this. However, there are three different types of tolerances. These are Relative, Nominal and Geometric. If we say that the correct answer at quiz time is calculated to 200 and the tolerance is set to 0.5 then the different tolerance types work like this:

Relative: A tolerance interval is calculated by multiplying the correct answer with 0.5, ie in this case we get 100 so for this tolerance the correct response must be between 100 and 300. (200 ± 100) This is useful if the magnitude of the correct answer can differ greatly between different wildcard values.

Nominal: This is the simplest tolerance type but not very powerful. The correct response must be between 199.5 and 200.5 (200 ± 0.5) This tolerance type can be useful if the differences between different correct answers are small.

Geometric: The upper limit of the tolerance interval is calculated as 200 + 0.5*200 and is the same as for the relative case. The lower limit is calculated as 200/(1 + 0.5). The correct response must then be between 133.33 and 300. This is useful for complex calculation that must have great tolerances where relative tolerances of 1 or more would be used for the upper limit but clearly not acceptable for the lower limit as it would make zero a correct answer for all cases.

The field Significant Figures does only relate to how the correct answer should be presented in the review or the reports. Examples: If it is set to 3 then the correct answer 13.333 would be presented as 13.3; 1236 would be presented as 1240; 23 would be presented as 23.0 etc. 


Page 2. Choose dataset properties
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Each wildcard that you specify in the answer formula must have an associated set of possible values - this is its dataset. Each of the wildcards is listed on this page along with a choice of dataset:

  * **private** i.e. only used by this question
  * **shared** i.e shared with other calculated questions in the same category 

Using a shared dataset can save time when you are creating a lot of similar calculated questions.

Note that even when creating a question for the first time, this page may say that your wildcard "will use the same existing private dataset as before." This just means that Moodle has already tentatively created a private data set for that wildcard: if a private dataset is what you want, leave this choice selected.

If there is anything in the question text that looks like a wildcard, but does not appear in any of the answer formulae, you can specify whether or not this is meant to be a wildcard. If it is, you can choose whether it should use a private or shared dataset.

To continue, simply choose your preferred dataset for each wildcard, then click "Next Page". 


Page 3. Edit the datasets
^^^^^^^^^^^^^^^^^^^^^^^^^^^
Now we need to create the set of possible values that each wildcard can take. Warning - this page is a bit confusing!

There are two ways of creating values - you can type them in yourself and add them to the list, or you can have Moodle generate them for you. 

**Adding/deleting your own values**

*Adding individual values to the list is easy:*

  1. In the 'Param' field for each wildcard, enter the value you want
  2. Scroll down to the 'Add' section and click the Add button (leaving the number of items set to 1)
  3. Repeat the above steps as many times as necessary (the maximum number of items is 100) 

*To delete values from the list:*

  1. In the 'Delete' section, select the number of items to delete
  2. Click the Delete button 

*Letting Moodle create values*

  1. Start with the "Range of Values" fields, and enter the lower and upper limits for the values you would accept
  2. Choose a number of decimal places for the value
  3. Choose the distribution of values between the limits - 'uniform' means any value between the limits is equally likely to be generated; 'loguniform' means that values towards the lower limit are more likely.
  4. Now move down to the 'Add' section and click on "force regeneration"
  5. In the menu next to the Add button, choose the number of sets of random values (items) you wish to add to the list. (Note that the maximum total number of items in your list is 100.)
  6. Finally, click Add to append the new values to the list
  7. **Note:** If you want more control over the items that Moodle adds, you can do them one at a time and preview the values before you add them. Click the "Get New Item to Add" button to make Moodle generate new values in the "Item to Add" section at the top. If you like them, click "Add" for 1 item; if not, click "Get New Item to Add" again to get new values. 

**Finishing off**

Once your list of items (values) is complete, you are finished. It's up to you how many values you add - the more values you add, the more a question can be used by the students without them seeing the same values repeatedly.

Note that if you delete values from the list, you can put them back again. Change the "Next Item to Add" option to "reuse previous value if available", then the next time you add items, Moodle will restore your previously-deleted items from the dataset.

Once your list of values is complete, you can click 'Save changes' to finish. 


Correct answer formula syntax
-------------------------------

DO NOT PUT THE = sign in the formula.
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  * In the recent versions of the calculated question type, you could have more than one answer formula and applied a specific grading value to each of them as long as there is at least one 100% correct answer formula. 

+------------------------------------------------------------------------------------+
| If more than one correct answer formula input fields are displayed when editing,   |
| your site has the mulyiple answer feature.                                         |
+------------------------------------------------------------------------------------+

  * As a general rule, write these formulas like you would in a calculator e.g. 3 + 5 * sin(3/{x}) A notable exception is exponentiation, where x3 cannot be entered as {x}^3, but instead should be entered as pow({x}, 3).
  * Each function's placeholders and other arguments should be in parentheses (brackets). For example, if you want students to calculate the sine of one angle and cosine of two times another angle, you would enter sin({a}) + cos({b}*2) or sin({a}) + cos(2*{b}).
  * It's usually better to have too many parentheses (brackets) than too few. The server won't care, and the more specific you are about what you mean, the more likely it will like your complex formulas.
  * There is no implicit multiplication. To you, the human editor, "5(23)" or "5x" may seem perfectly obvious. To the server doing the math, it's crazy talk and won't be understood. Always use the "*" for multiplication.
  * Any special mathematical function must have parentheses around its values. Take the sine function in the first bullet point for instance. Notice that the 3 / x is wrapped in parentheses (brackets)--this is so the server can understand it properly. Without those parentheses, the server won't know if you mean "(sin 3) / x" or "sin (3 / x)" and will reject the entire formula accordingly. 

Predefined constants
^^^^^^^^^^^^^^^^^^^^^
Actually there is NO Predefined constant that is allowed other than pi() as a function without parameter. 

Synchronization
^^^^^^^^^^^^^^^^
You could use shared wild cards to get the same values across questions in a quiz.

A simple example will be to use the same radius in a first question asking for the perimiter of a circle of {radius}cm and a second question asking for the surface of a circle of {radius}cm.

When the quiz will be shown to the student the two questions will shown the same {radius} value.

However the synchronization will work **ONLY** if the questions are kept in the **SAME** category and have the **SAME NUMBER OF DATASETS** .

If you need to move the synchronized questions to another category, you need to do it by editing the questions. 



















