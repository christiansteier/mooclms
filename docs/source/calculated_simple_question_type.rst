.. _calculated_simple_question_type:

Simple Calculated question type
================================
Simple calculated questions offer a way to create individual numerical questions whose response is the result of a numerical formula which contain variable numerical values by the use of wildcards (i.e **{x} , {y}**) that are substituted with random values when the quiz is taken.

The simple calculated questions offers the most used features of the calculated question with a much simpler creation interface. 

My first Simple calculated question
-------------------------------------
As a first example you will create a question asking for the surface of a rectangle. Here are the quick steps we will go over in detail:

  * Create the question content with variables shown in {}
  * Enter the formula using the variables and set the tolerance
  * Determine the range of the generated set of variables that will appear in the question content
  * Review the generated set of question contents
  * Since it is your first, check your work from a student's view 
  
1. Initiating the creation process
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Go to the Question bank, select "create a new question" and in the pop-up window select the Simple calculated. The Simple calculated question interface will appear. Give a name to your question in the title. 

2. The question text
^^^^^^^^^^^^^^^^^^^^^
Fill the question text (note that the {param} names can be chosen at will. 

3. The Correct Answer Formula
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Fill the Correct Answer Formula using the {param} names used in the question text. 

4. Other answer and response parameters
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
You will set the Grade to 100%, as this is the only answer in this question.

Leave the other parameters as they appears ( 0.01 relative means ±1% tolerance). 

5. Find the {param} in the formula
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
In simple calculated only the {param} that are in the formula will be used.

In the question text , the {param} that are in the formula will appear with there numerical values i.e 6.7 .

Any other {enclosed text} will appear as is i.e. {enclosed text}. 

**Click on the button**

On reload the two {b} and {h} will be displayed. 

Set the minimum and maximum values
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Here the {b} range has been set to a 15-20 range and the {h} range has been set to a 5-10 range as we want a rectangle with a larger base than height. 

Select the number of sets to generate (here 10) and to display(here 2)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Just to illustrate that you can control the number of values displayed which is useful if you create 100 sets.

Also note the (red) warning that a valid question needs at least one set of {wild card} values. You will not be allowed to save the question if you don't do the next step.

Click on the generate button
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Note the sets are shown in reverse order so the the number indicates how many sets were created.

The two sets illustrate that the variability defined by the Min and Max values.

Note that the formula result is analyzed and the tolerance limit (here 1% relative) is shown

The correct response that will be shown to the student is also shown.

The 2 decimals where defined are the default values defined as the last parameter under the Correct formula. 

Click on the Save button

Test your first Sinple calculated question

On the question bank click on the preview icon.

Enter the result you have calculated yourself or click on the Fill with Correct button.

The values should be identical... 



















