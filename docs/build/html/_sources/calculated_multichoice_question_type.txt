.. _calculated_multichoice_question_type:

Calculated Mutichoice question type
====================================
Calculated multichoice questions are like multichoice questions with the additonal property that the elements to select can include formula results from numeric values that are selected randomly from a set when the quiz is taken. They use the same wildcards than Calculated questions and their wildcards can be shared with other Calculated multichoice or regular Calculated questions.

The main difference is that the formula is included in the answer choice as {=...} i.e if you calculate the surface of a rectangle {={l}*{w}}.

The value will be displayed as set by the **Correct answer shows** (0,1,2 etc) and **Format** (decimals, significant figures).

So a Choice text could be

The rectangle surface is {={l}*{w}} cm2.

If {l} = 4,0 , {w} = 2,5 , **Correct answer shows** 1 and **Format** decimals

The choice will display as

The rectangle surface is 10.0 cm2 

Handling of the wild cards, and the available functions is similar to the calculated question type. 
