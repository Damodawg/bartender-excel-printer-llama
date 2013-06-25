excel-taktclock-bartender-VBA-Autoprinter-llama
=============================
**this was submitted as a code sample for a Code Fellows application.  The working version did not use the takt clock - ie
I didn't get around to implementing this version, so in a CYA move, there are likely some bugs in the bed. 

This code runs with a specific userform.  The entire package can be found and downloaded here.  Enable all content. 
https://docs.google.com/file/d/0BwDr8PN7RrULQXVSTHJvdWJCSVU/edit?usp=sharing

Why did I create this?
I created this program because production workers were spending ~30 sec to 1 min manually selecting parameters and printing labels.
In a high volume production system, this adds up to serious $ and time.  With this program, this process takes less than 2 sec
for most labels. 

What does this do?  
This is a program which would be used in a one person production cell to monitor progress, automate printing
and keep production at a certain speed (on takt).  Here's a wiki page on takt time http://en.wikipedia.org/wiki/Takt_time .  In summary
takt is the amount of time a station has to complete its work in order to satisfy the rate of customer demand.  

Users login, and hit start.  This program was designed to automate printing and show a visual of how ahead or behind they
are in their day. The TM's goal is displayed and it tracks how many units have been completed.  Admin's can edit the goal
in the spreadsheet "Goals".  In addition, Admins can monitor the progress and run reports/stats on the data provided in 
the datadump, which logs events.  

Because this was intended to run on a touchscreen, the UI is big and bulky.  The user can toggle between different 
labels by clicking the button which initially says "Norm" (aka normal).  WWG labels were intended for Grainger orders 
which uses a different format.

Labels are presented based on reading the matrix in the model info spreadsheet. 

Worksheet 1 & 3 WERE linked to an internal, company specific label database.  

This highly customized program utilizes bartender api calls and will not run properly 
without proper bartender software and templates

Links are hardcoded and unless pigs fly, will not work properly
on machines other than the machine that this was intended to run on

Created by Damodawg, Enjoy! 
