.. _import_glossary_entries:

Import glossary entries
========================
Glossary entries can be exported and then imported into another glossary via an XML file. 

  * As an editing teacher, access your glossary.
  * Go to *Administration > Glossary administration > Import entries*. 
  * Click the "Choose a file" button and browse for the exported entries XML file on your computer
  * Select the destination for the new entries: either the current glossary or a new one
  * If you want to import category information, click the checkbox.
  * Click the "Submit" button. 

You'll then see a report of the entries and categories added to the glossary. If you enabled duplicate entries when you created the glossary, the import process will add all of the new definitions. Otherwise, it will not allow you to import any duplicate entries.

You will be listed as author of all the entries. 

Troubleshooting
----------------
Possible causes of problems importing entries:

  * If there are mistakes in the XML file such as the <entries> tag being missing or the <info> tag being in the wrong place. May happen if you have constructed the XML file manually or with some sort of tool like mailmerge in Word and your template is wrong.
  * If there are top bit set characters in the text of the entities like concepts, definitions or keywords. Replace things like & with &amp;
  * If there are tabs or spaces between entries. Not sure if spaces cause problems but best to remove any between the end of one tag and start of the next. e.g. Search and replace > < with >< via a text editor.
  * In most cases the import is halted if any of these errors occur.
  * Duplicates in the entries which clash with entries already when merging a glossary is usually not a problem.
  * Warnings like Warning: exec() has been disabled for security reasons in /moodle/lib/uploadlib.php on line 603 may not be the problem when importing but may distract one from dealing with problems with the format of the XML file.
  * HTML and XHTML tags written within CONCEPT or DEFINITION elements will fail on import, showing "Array" instead of the desired content. To remedy this, try writing the (X)HTML tags within <![CDATA[ ]]> markup.
  * If the glossary entries contain images, image paths will need amending by doing a search and replace in the XML file in order for the images to be displayed when the file is imported. 
  
Restoring a glossary activity backup
--------------------------------------
An alternative method of importing glossary entries is to restore a glossary activity backup containing enrolled users. This method includes categories, images and attachments within glossary entries. When the glossary is restored, the authors of the entries will be the same as in the original glossary. 

