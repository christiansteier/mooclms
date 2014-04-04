.. _export_questions:

Export questions
=================
Questions may be exported from the Quiz module and the :ref:`Question bank <question_bank>` in any one of 3 formats:

  * GIFT format
  * Moodle XML format
  * XHTML format 

In addition, questions may be exported into Word format using a contributed plugin, :ref:`Word table format <word_table_format>`. These can then be easily used to create paper tests.

Process
--------
  * Click *Administration > Quiz Administration > Question bank > Export*. 
  
  .. image:: _images/export_questions.png
  
  * Select the output type required for the exported file.
  * Use the pulldown menu to select the question category you want to export
  * Check if you want the category name to exported and/or the context to be included. This only applies to some formats and is used to restore this information on import.
  * Click on the export questions to file button
  * You are invited to download the file to your computer. 
  
Example uses of exported files
--------------------------------
  * GIFT and Moodle XML formats can be imported into the Lesson module And Question bank via an import question process.
  * Exported question files on one server, can be imported into another Moodle site/server
  * GIFT and Moodle XML formats can be tweaked to create word processing or spreadsheet documents suitable for paper tests or vetting.
  * In case you want to convert your Moodle XML file into text format upload XML to http://moodle.heroku.com. It automatically generates *.txt with your questions.
  

.. _word_table_format:

Word table format
------------------
Moodle2Word is a Moodle 1.9 and 2.x add-on that allows question banks to be exported from Moodle into a Word file. The Word file can then be used to quickly review large numbers of questions (either online or in print), or to prepare paper tests (where the answers and feedback is hidden). Questions in the Word table format can also be imported into Moodle. 

Features
---------
  * The tables contain all components of a question, including the stem, answer options, option-specific and general feedback, and any images.
  * All the main question types except Numerical and Calculated questions are supported.
  * With the aid of commands in an external Word template, questions can be re-formatted to hide the answers etc, allowing the questions to be printed as a paper quiz.
  * Questions can be edited in Word, and then imported back into Moodle.
  * The Cloze question syntax for importing questions is very simple, as it does not require any knowledge of the arcane Moodle syntax; instead, use bold for drop-down menu items, and italic for fill-in text fields.
  * The plug-in supports import from and export to all languages, not just English.
  * Equations created using MathType or the built in Microsoft Equation Editor are converted into images on import.
  * Questions can be quickly previewed in Moodle, as you are creating them.
  * New question features added in Moodle 2.x, such as Hints and Tags, are supported. 


  
