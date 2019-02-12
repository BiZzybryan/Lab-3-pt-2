# Lab-3-pt-2Lab - Working With Files
==========
Follow the instructions line-by-line.  

* Type in the commands as is, but ignore the beginning prompt.  
* Enter, tab, up and down are represented by <ENTER><TAB>,<UP> and <DOWN>.  
* "No output" or "nothing happens" are valid answers to any of the questions.
==========

==========
1. Open a new terminal window.
[NO OUTPUT]
----------
==========
2. Find out if mtec1003-lab-03 already exists (from the previous lab).  If it doesn't, go back to the previous lab and find the steps regarding downloading the lab materials.

(See steps 1-8 in http://entertainmenttechnology.github.io/Wilson-MTEC1003/labs/03/lab-03-part-01-review.txt)
[NO OUTPUT]
----------
==========
3. Change your directory mtec1003-lab-03
[NO OUTPUT]
----------
==========
4. Create a directory called my_files
[NO OUTPUT]
----------
==========
5. Change the directory to my_files
[NO OUTPUT]
----------
==========
6. Create a new file using touch.

$ touch foo.txt
$ ls
Copy and paste the output below.
----------ls
foo.txt



==========
7. Create another new file using touch.

$ touch bar.txt
---------- touch bar.txt
V217-M11:my_files bryan.pierrelouis02$ 


==========
8. List the files in this directory using the flag that gives the most details.

Copy and paste the output below.
----------total 0
-rw-r--r--  1 bryan.pierrelouis02  ACADEMIC\Domain Users  0 Feb 11 19:51 bar.txt
-rw-r--r--  1 bryan.pierrelouis02  ACADEMIC\Domain Users  0 Feb 11 19:51 foo.txt

==========
9. Create a copy of bar.txt called baz.txt and then list the files again.


Write the command that you used to copy the file.  Additionally, copy and paste the output of your file listing below.
----------total 0
-rw-r--r--  1 bryan.pierrelouis02  ACADEMIC\Domain Users  0 Feb 11 19:51 bar.txt
-rw-r--r--  1 bryan.pierrelouis02  ACADEMIC\Domain Users  0 Feb 11 19:53 baz.txt
-rw-r--r--  1 bryan.pierrelouis02  ACADEMIC\Domain Users  0 Feb 11 19:51 foo.txt


==========
10. Delete the file called bar.txt and then list the files again.

Write the command that you used to remove the file.  Copy and paste the output of your file listing below.
----------total 0
-rw-r--r--  1 bryan.pierrelouis02  ACADEMIC\Domain Users  0 Feb 11 19:53 baz.txt
-rw-r--r--  1 bryan.pierrelouis02  ACADEMIC\Domain Users  0 Feb 11 19:51 foo.txt==========

11. Move the file called foo.txt to qux.txt and then list the files again.


Write the command that you used to move the file.  Copy and paste the output of your file listing below.
-----------rw-r--r--  1 bryan.pierrelouis02  ACADEMIC\Domain Users  0 Feb 11 19:53 baz.txt
-rw-r--r--  1 bryan.pierrelouis02  ACADEMIC\Domain Users  0 Feb 11 19:51 qux.txt


==========
12. Go up one directory so that you're in ~/mtec1003-lab-03.
[NO OUTPUT]
----------



==========
13. Try removing the directory called my_files using rmdir.

Write out the command that you used and what happened.
---------- bryan.pierrelouis02$ rmdir my_files
rmdir: my_files: Directory not empty



==========
14. Try removing the directory called my_files using rm.

Write out the command that you used and what happened.
----------rm my_files
rm: my_files: is a directory



==========
15. MAKE SURE YOU'RE IN THE mtec1003-lab-03 directory!  

Force the removal of the directory and files using the -rf flag

$ rm -rf my_files
----------rm -rf my_files
V217-M11:mtec1003-lab-03 bryan.pierrelouis02$ ls -l
total 1552
-rw-r--r--    1 bryan.pierrelouis02  ACADEMIC\Domain Users  794624 Feb 11 19:45 access-0.log.tar
drwxr-xr-x@   5 bryan.pierrelouis02  ACADEMIC\Domain Users     160 Feb 11 18:57 books
drwxr-xr-x@ 129 bryan.pierrelouis02  ACADEMIC\Domain Users    4128 Feb 11 18:25 logs
drwxr-xr-x@   6 bryan.pierrelouis02  ACADEMIC\Domain Users     192 Feb 13  2013 web


==========
16. There's a txt file version of a book located in the mtec1003-lab-03 folder.  It is in the following directory if you're in the lab folder:

books/other/pg1232.txt

Use the command called cat on the file to show its contents. 

Describe what happened below.
---------- The entire "pg1232.txt" opened up a story and its extremely long.


==========
17. That was a lot of text.  Let's find ways to limit it.  Using the same file...

books/other/pg1232.txt

Use the command, head, on the file to show the contents of the beginning of the file.  

Write the command that you used below.  Write the last line of the output below (it should be the title).
----------The Project Gutenberg EBook of The Prince, by Nicolo Machiavelli

This eBook is for the use of anyone anywhere at no cost and with
almost no restrictions whatsoever.  You may copy it, give it away or
re-use it under the terms of the Project Gutenberg License included
with this eBook or online at www.gutenberg.org


Title: The Prince



==========
18. Using the same file again!

books/other/pg1232.txt

Use tail on the file to show the contents of the end of the file.  

Write the command that you used below.  Write the last line of the output below.
----------Most people start at our Web site which has the main PG search facility:

     http://www.gutenberg.org

This Web site includes information about Project Gutenberg-tm,
including how to make donations to the Project Gutenberg Literary
Archive Foundation, how to help produce our new eBooks, and how to
subscribe to our email newsletter to hear about new eBooks.



==========
19. Using the same file...

books/other/pg1232.txt

Use less and more on the file to show the contents of the file.  Try pressing spacebar and/or q afterwards.

Write the command that you used below.  Describe what spacebar and q does after using either less or more.
----------
the spacebar displayed the entire story again.


==========
20. Describe what situations you would use the following commands for viewing files: less, more, cat, tail, head

(Some characteristics that may help your description might be the length of the file, whether or not you'd like to read the whole thing... or just the beginning or end, etc.)
---------- Situations when a file is too much to scroll down to the end, you could use 'tail' to see the end with no problem or head to see the top of something easier.

The command cat could be used to display a file easier without having to go to the file in finder for yourself.


==========
21.  How many words are in pg1232.txt?  What command did you use to determine the word count?
----------



==========
22.  How many lines are in pg1232.txt?  What command did you use to determine the line count?
----------


==========
23.  Make sure you're in the books/other folder.  Copy all of the txt files from that folder to your home directory using wildcard matching.

Write the command that you used below.
----------
