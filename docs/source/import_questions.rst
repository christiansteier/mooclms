.. _import_questions:

Import questions
=================
Moodle has a number of different formats that can be used to import questions into :ref:`Question bank <question_banks>` categories and as lesson question pages. These include some proprietary quiz software formats, as well as text files and Moodle formats.

Importing questions from an existing file
-------------------------------------------
It is possible to import questions from a file on your network/computer or from a file that has been saved or uploaded into your course files. The underlying character encoding of this file is important.

**Note:** Moodle XML format is the recommended import question type format as it enables the maximum amount of question data (such as question feedback) to be imported. 

Question bank import process
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The question bank allows you a great deal of flexibility when importing questions. To import questions into Moodle's Question bank, use the Questions link in the course administration and select the import tab. In most versions of Moodle it is also possible to get to this screen (produced by ../question/import.php) while editing an existing quiz. 

  * Select import tab
  * Select the question type to import
  * General: pick the category, determine if the context and category information that maybe contained in a GIFT or XML file should be used.
  * Select what should happen if there are no grades or an error is detected in the import process.
  * Determine the file to import
      * Import from file upload. Use the browse function to import a file from your computer. Use the "Upload this file" button to import the questions.
      * Import from file already in course files. A popup window will take you to the course files start page. Use the "Import from this file" button. 

Lesson moule process
^^^^^^^^^^^^^^^^^^^^^
The question types that can be imported from the Quiz questions bank into a lesson are the following: Matching, Multichoice, Numerical, Short answer, True/false.

The Description and Cloze questions can **not** be imported from Quiz questions bank into a lesson.

Lesson can only import from a file located on the teachers computer.

  * In edit, using the expanded view
  * Select the position where questions should be inserted into the lesson
  * Click on the Import question link between the pages.
  * Select the file type
  * Use the browse function to find the file on your computer
  *Import the selected file. 

Questions import formats
^^^^^^^^^^^^^^^^^^^^^^^^^

GIFT
^^^^^
Moodle 'proprietary' text format for import and export. Reasonably comprehensive. 

Moodle XML
^^^^^^^^^^^
Moodle 'proprietary' xml format for import and export. Very comprehensive. 

Aiken
^^^^^^
This format is an easy way of writing multiple-choice questions for import. 

Blackboard
^^^^^^^^^^^
It's possible to import both .dat files containing just questions text or zip archives containing questions and associated medias (images, sounds, ...).

If your questions contains images they are imported too.

Also both Blackboard POOL and QTI files are supported.

Questions produced with TestGen and Examview softwares and saved as Blackboard files are imported.

If the zip archives contains several resources files all questions from all files are imported. "Undeployed" Blackboard quiz are also supported.

Follow these steps to import questions:

1. Create a quiz with questions in Examview Test Generator v. 6.2.1 or another question generator able to save questions as Blackboard files like TestGen.

2. Export the quiz to Blackboard 6.0-7.0 format.

3. From the Settings tab for your course choose Question bank and then Import. Make sure you use the Blackboard format.

**NOTE:** Some tutorials on the web explain that you need to edit files to re-link images. This is no more needed. Images are imported without any editing.
Importing questions in different categories

If you check the "Get category from file" option during import, the category name for each resource file will be extracted for the resource file and created if necessary.

If "Get category from file" is unchecked, all questions will be imported in the current category.

Embedded Answers (Cloze)
^^^^^^^^^^^^^^^^^^^^^^^^^
This format is a multiple question, multiple answer question with embedded answers. They can be a bit tricky to develop, but they are a unique way of asking questions. 

Examview
^^^^^^^^^
ExamView 4 supported an XML export format that Moodle can import.

Follow these steps to import questions from ExamView 4.0.8

1. Create a new test using ExamView

2. After selecting the types of questions and how many of each Click on File - Export – Change Save As Type to ExamView XML

3. After creating the export of your ExamView test login to your Moodle site

4. Go to the course you wish to add the quiz to and Turn Editing On

5. Scroll down to the topic or week you wish to add a Quiz Click add an activity – highlight quiz, Enter a name and introduction for the quiz and any other applicable information.

6. Click save and display

7. Editing quiz - click Edit then Import, click the radio button next to ExamView

8. Browse to the location you saved the file highlight and click open, then click the upload this file button.

9. Review the questions imported, click continue, click on Quiz, select all and click add to quiz

10. Save Changes, click on the preview tab view the test and the quiz is ready.

If you are using a newer version of ExamView, you should export your questions from Examview choosing the Blackboard format:

1. In ExamView choose one of the two Blackboard export options, either Blackboard option can be imported into Moodle, however it is recommended to choose the Blackboard 7.1+ option

2. Save the zip archive ExamView creates

3. Import this zip file in Moodle using "Blackboard V6+" format. see the above paragraph about the Blackboard V6+ import format for more informations. 


Learnwise
^^^^^^^^^^
This format can import multiple choice questions saved in Learnwise's XML format.

Missing word
^^^^^^^^^^^^^
This format is only used for multiple choice questions and short answer questions, similar to GIFT.

WebCT format
^^^^^^^^^^^^^
This format supports importing multiple choice and short answers questions from WebCT's text format.

**Caution:** Keep in mind that WebCT allows more than one "blank" per short answer question; whereas, Moodle will only accommodate one blank per question. Questions that used multiple short answers in a question will not convert successfully.

Word table format
^^^^^^^^^^^^^^^^^^
This format supports importing all question types (except calculated) from structured tables in Microsoft Word files. Creating, editing and managing large numbers of questions is much easier in an external Word file than maintaining them one at a time inside Moodle. 


Hot Potatoes
-------------
A freeware program that can export questions into Moodle.

**Note 1** - All types of Hot Potatoes question types can be imported into Moodle, but JCross and JMix questions will be changed to Short Answer questions.

  * Can be imported into the Quiz questions bank:
      
      * Cloze questions (JCloze);
      * Match questions (JMatch);
      * Multiple Choice questions (JQuiz)
      * Short Answer questions (JQuiz, JCross and JMix) 

  * Can be imported into Moodle's Lesson module:
     
      * Match questions (JMatch);
      * Multiple Choice questions (JQuiz) 

**Note 2** - For Hot Potatoes' Multiple Choice question type (JQuiz), the Multiple-choice Short answer and Multi-select question-type will imported as they are. Hybrid questions will be imported as MultiChoice questions, i.e. they will not start as Short Answer questions and then change to Multiple Choice questions after several wrong responses. 

Importing from other programs
------------------------------

Diploma 6
^^^^^^^^^^
Diploma 6 also supports an XML export format that Moodle can import. If you are using a newer version of Diploma, here are the steps to export from Diploma and import to Moodle. The steps are the same as those for Blackboard(see above).

  * Export from Diploma with the Blackboard LS 6.0 – 6.2 format.
  * Import the .zip file using the Blackboard format. The images are imported at the same time. 

Old formats
^^^^^^^^^^^^
AON -This format is the same as the missing word format, except it creates matching questions from the multiple choice questions. Please note that from Moodle 1.8 it will no longer be part of the standard Moodle. 






