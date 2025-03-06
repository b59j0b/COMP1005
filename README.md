java c
COMP1005 B Winter 2025 – “Introduction to Computer Science I” 
COMP1005 B 
Assignment #3 
Functions, Strings,   Files 
Overview 
In this assignment, you will demonstrate your understanding of (in   addition   to   previous   topics):
•    Reading and writing text files   in   Python
• Performing   string   operations   (like   strip   (),   split   ())
• Appending data to lists and checking   if elements are   in   lists   using   in
•    Defining and using your own functions which accept   parameters   and   return   a value   This assignment   has 40 marks and 4 bonus marks available.
Submission Requirements 
Submit   a   single zip file with   the   name   comp1005__a3   .zip   (comp1005 or   comp1405 both acceptable) to   Brightspace. This   zip   file   should   contain two Python files named   assignment3   .py   and a3_tester   .py, both of   which are initially provided to you on Brightpace   in   comp1005-a3-starter   .zip, and any   flowcharts completed for bonus   marks. 
Standard Assignment Policies 
Late Submissions: Submissions can   be accepted late without   penalty   until   Sundays   at   11:59PM,   but   later   submissions will   not   be accepted. Support will   not be provided   during this   late   period.Technical issues near the deadline are not grounds for extension. You are   expected to   submit frequently throughout the time the submission is available and   use   the   School   of   Computer   Science   computer labs   if necessary.
Incorrect submissions are not grounds for extension. It is your   responsibility to   download   and   review   your submission prior to the submission cut-off period and verify   that   you   have   followed   the   submission requirements. Review the course outline for more information 
Academic Misconduct 
Submissions will be automatically compared to each other and   then   any   suspiciously   similar   code   will   be   manually reviewed.   Any code that seems suspiciously similar will   be forwarded to the   Dean’s   office   for further investigation. You are not permitted to collaborate with other students   by sharing   rough work   or code. You are not permitted to use chat or   codegenerative   AI to   assist with   creating   rough   work,   written explanations, or code.   In   no way should you pass off the work of others   as   your   own   or   assist   others   in doing the same.   Review the course plagiarism policy for further   information.
Note: Use of official documentation or the course textbook and course   notes   are   permitted.   Simple   citations,   such as   including links or references to the   course textbook   or   official   Python   documentation   are   advised   if any work is copied from these   sources.
Invalid Submissions 
Submissions containing incorrect packaging, naming,   or file types will   receive   an   approximately 10% penalty with   no exceptions. To dispute the grade once grades   release, you   have seven days to   contact   the   TA that   marked you with   information about what was marked incorrectly. 
Assignments 3 Specification | Due Fri, Mar. 07 @ 17:00 
Job Posting (Assignment Overview) 
Note: This is not a real job posting but optional context for the assignment. Feel free to skip this if you would prefer to focus on the technical requirements. 
Job Title:   Paranormal   Instrument Software   Designer
Duties:   Developing the   software for ghost hunting equipment
Requirements:   Experience with lists, strings, reading and writing files, and   defining   functions
Description: We’re the   Raven Ghost   Hunting Society (RGHS) and we’re   looking for   someone   to   help automate the analysis of our sensor readings. We go to   abandoned   houses   and take   sensor   readings with   various devices to try and detect ghosts! Our sensors   output   their   data   to files,   and   each   sensor   uses   a slightly different file format.
We   need you to write a program that can   read sensor   data from   our   three   different   sensors,   process   that   data, and output whether or not   it’s abnormal.   If a   room   has   abnormal   readings   in   more than   one   sensor,   we’re DEFINITELY dealing with some kind of entity! We   previously   hired an   intern to   write   some   testing code, but they were so terrified of the thought of slightly cold   temperatures   and wifi   signal   interference   that they ran off before finishing anything, so you   have   somewhere to   get   started.   Good   luck!
Provided Code 
You   should   begin   by   downloading   and   extracting   the   files   in   comp1005-a3-starter   .zip.   It   contains:
•   assignment3   .py: This   is   the   starting   point   for   writing   your   code.   A   few   of   the   functions   have   been   setup   for you   to   get   started,and   they   use   type   hints   and   are   documented   to   get   you   started.
•   a3_tester   .py: You   do   not   need   to   read   this   code.   It   contains   some   testing   functions   which   you   (and   the TAs) can   use to test   how your code   is doing as you write   it.   As   long   as   the   test   text files   and   the   Python   files are all   in the same directory, you can   run this   Python   program   to   see   how   things   are   doing.
•    ravensnest   .*   .txt: There   are   three “ravensnest” files   which   can   be   used   for   some   simple   testing   of   your program   to   see   how   the   program   works   in   context. This   is   what   your   assignment3   .py   should   test   with.
•   test   .*   .txt: There   are   three “test” files   which   are   used   by   the   a3_tester   .py   program.   They   contain   a   bunch of tests, and locations specifically named after different   situations where   your   code   might fail.
• report_test   .*   .txt: There   are   three “test” files   which   are   used   by   the   a3_tester   .py   program   used   to   test correct generation of reports.
Functions to Write 
A   fully   completed   assignment3   .py   should   include   the   following   functions, all   with   the   correct   naming,   returning the correct return values, and accepting the   correct   parameters:
1.   main   ()   which returns nothing and handles the   main   control flow   of your   program.   It   should   be   quite   simple   and   run   your   functions   with   the   ravensnest   location   data.
2.    read_motion   (),   read_emf   (),   read_temperature   ()   will all open files based on the provided location name   and   return a list of “abnormal” rooms. The start   of these   has   been   provided.
3.   get_unique__rooms   ()   accepts   three   lists   of   strings   containing   the   rooms   that   were   considered “abnormal”   by the   previous three functions and   returns a list of   rooms that   appeared   in   at   least   one   of   each, without duplicates.
4.   generate_report   ()   accepts   a   location   name   as   a   string   and   three   lists   of   strings, the   rooms   that   were considered “abnormal” by each sensor function, and   returns   nothing.   It   identifies which   “ghosts”   must   have appeared   in each   room   in the location and writes this   report to   a   file.
Bonuses Available 
Reminder: The maximum mark for the overall assignment   portion   (all   assignments   combined)   of your grade   will   not exceed   100%,   but   bonus   marks on each assignment can   help   bring   up   lower marks   on   other assignments.
Flowcharts (2 marks) 
To   begin, you should try to   make a   plan for how you will   analyze   each   problem. You   can   receive   2   bonus marks for including a flowchart for each of   read_motion   (),   read_emf   (), and   read_temperature   ()   if you submit   a flowchart that shows your plan for reading the data   in   each   room   and   storing   the   appropriate   list   of   rooms.   The flowcharts do   not   need to   be   perfect; just sketch your control flow   in a way the TA (and you!)   can follow. Include these flowcharts as one or more PDF, PNG, JPG files in   your zip   submission. 
Read Ahead: Exception Handling (2 marks) 
When working with files, it’s very easy for things to go wrong;   incorrect file   names,   not   being   allowed to   open   a file, or already   having a file open - to   name a   few. Exceptions are   signals   that   some   situation   cannot   be easily   handled. Chapter 13 of   the   textbook   discusses   exceptions   using   try..except. This   tool   lets   us   choose to run some code that could go wrong,   and   rather than   crashing   our   program,   continue   it   gracefully.
In   your   main   ()   function, allow   the   user   to   specify   which   location   they   want   to   investigate   using   input   ()   rather than   hardcoding   the   name   of   the   filename. Then, in   each   of   your   read   functions   (   read_motion   (),   read_emf   (),      read_temperature   ()), use try   and except   when opening the file so that if an invalid   location   is sent   and the file cannot   be opened,   it will   provide an appropriate error message   and   return   an   empty   list   of   rooms   instead   of crashing.   For marks, the TA must   be able to   input the   name of valid and   invalid   locations,   and   for   invalid locations, get a   message telling the that the file cannot   be found, and   try/except   must   be   used   in   those   three   functions.
Problem 1-3 Overview 
Problems   1 - 3 are very similar in their   structure.   To   avoid   repetition,   here   are   a   few   notes   which   apply   to   them   all:
1.    Each function will   read data from a text file and   return a   list   of   rooms   considered “abnormal”, 
2.    Each function will accept a location   name as   a   string   and   open   a file   based   on   that   location.   For   example, for the location “house” passed into the   argument   location_name:
a.      Motion data will be found in   house   .motion   .txt   b.    EMF   data   will   be   found   in   house   .emf   .txt
c.   Temperature   data   will   be   found   in   house   .temp.txt
3.   A room should only appear at   most once   in the   returned   list
4.    Each function will   need to loop,   reading data   in line-by-line,   until   it   reaches   the   end   of the file.
5.    Update your main   ()   function to store the list returned   by   each   of these when   calling   them with   the argument   "ravensnest"   to   get   sample   data. You   can   print   it   out   to   test   if   it   worked.
6.    Running   a3_tester   .py   will   run   the   test   suite, with   lots   of   different   pieces   of   test   data   to   give   you   an   idea of how your functions   are going.
Use the documentation   in the   provided code to assist you   in filling   in any   knowledge   gaps   left   by   the   problem description.
Helpful Tools and Tips: Review the final   page for extra   information that   might be   helpful   for this   assignment.
Problem 1: Motion Sensor 
Submission: Update the function   read_motion   (location_name)   in assignment3   .py   and include this and any   bonus flowcharts in your zip file.
Context: The   motion sensor occasionally turns on to see   if anything   is   moving   in the   room and   reports “detected” if it notices motion or “undetected” if   nothing   moved.
Abnormal: Abnormal readings are readings where motion   is   detected   at   least   once.
File Format: Each   line   contains   the   name   of   a   room   followed   by   a   colon,   a   space,   and   either   detected   or undetected.
Example File: house.motion.txt
01      bathroom:   undetected
02      living   room:   undetected
03      living   room: detected
04      bathroom:   undetected
05      kitchen: detected
06      kitchen:   undetected
Example Expected Result: read_motion   ("house") # Returns   :["living   room"   , "kitchen"]
Process: Loop until reaching an   empty   line.   In each   loop,   use   split   ()   to   help   determine   if the   room should         be appended to the   rooms   list that you are returning or not.   Make   sure   not to   append   the   room   if the   rooms   list already contains the   room.
Problem 2: EMF Sensor (Electromagnetic Fields) 
Submission: Update the function   read_emf   (location_name)   in assignment3   .py   and include this and any   bonus flowcharts in your zip file.
Context: An   EMF sensor detects electromagnetic field fluctuations in an area,   such   as   those   produced   by   cellphones, radio代 写COMP1005 B Winter 2025 – “Introduction to Computer Science I” Assignments 3Python
代做程序编程语言s, or power lines. We will   measure this   on   a   scale   of 0 to   5.
Abnormal: Any room that has an average EMF   reading greater than or equal to 3 will   be   considered “abnormal” … for some reason.
File Format: A line contains either a   room   name or an   EMF   reading, as a whole   integer, for the   most   recently written room.
Example File: house.emf.txt
01      bathroom
02      1
03      2
04      1
05      living   room
06      5
07      4
08      2
Example Expected Result: read_emf   ("house") # Returns   :["living   room"]
Process: Design your own approach for this, but here   are   a few   useful   tips:
•   Strings   have   the   .isdigit   ()   method, which   returns   True   if   the   string   is   an   integer.   E.g.,   "4"   .isdigit   ()== True   and   "cat"   .isdigit   ()==   False
• Average: One   method to take an average reading for   each   room   is   to,   starting with   a   count   and   total   of   0,   add each   reading to your total sum and   increase count   by   1 each   time you   get   a   reading.   When   finished         with that room, get the average by   dividing   the   total   sum   by   the   number   of   readings.
• Rolling Average: Alternatively, you can   maintain a “rolling” average that   updates with   each   new value,  ,   with:
avgnew    = avgold   + n/x−avgold 
, where n is the total   number   of values so   far.
•   You will likely   need some variables to track what the current   room   is, what   the   current   count   and   average   are, and possibly   the   current   total.
• Remember: Depending on your method, make sure that   you   check   the   average   of the final   room   before   returning your function!   It’s surprisingly easy to miss.
Problem 3: Temperature Sensor 
Submission: Update the function   read_temperature   (location_name)   in assignment3   .py   and include this and   any bonus flowcharts   in your zip file.
Context: Temperature   is tracked   in celsius with real   numbers.   Anything below 0   is   considered   freezing,   where water freezes.
Abnormal: According to this club, any room that consistently   reads   temperatures   under   0.0 for   5   readings   in   a   row   is considered to   be an abnormal room. Who isn’t afraid of the   cold,   I   guess?File Format: This data   is stored as “Comma Separated Values”, a   very   common   format.   On   each   line,   you   will find the room name, a timestamp, and   a   temperature,   separated   by   commas.   The   readings   for   a   room      will always be   one   after   another.
Restriction: You are not permitted to include additional modules, such   as   the   csv   module, to   assist with   parsing this data.
Example File: house.temp.txt
01      bathroom   ,1700001   ,25   .3
02      bathroom   ,1700002   ,25   .1
03      bathroom   ,1700003   ,24   .3
04      bathroom   ,1700004   ,26   .1
05      bathroom   ,1700005   ,-10   .4
06      bathroom   ,1700006   ,25   .3
07      bathroom   ,1700007   ,24   .8
08      garage   ,1701200   ,30   .1
09      garage   ,1701201   ,20   .5
10      garage   ,1701202   ,-5   .1
11      garage   ,1701203   ,-2   .4
12      garage   ,1701204   ,-10   .1
13      garage   ,1701205   ,-5   .0
14      garage   ,1701206   ,-20   .1
15      garage   ,1701207   ,-9   .1
16      garage   ,1701208   ,10   .4
17      garage   ,1701209   ,26   .5
18      kitchen   ,1700030   ,25   .0
19      kitchen   ,1700031   ,24   .5
20      kitchen   ,1700032   ,-10   .4
21      kitchen   ,1700033   ,30   .4
22      kitchen   ,1700034   ,28   .7
Example Expected Result: 
read_temperature   ("house")
#   Returns   : ["garage"]
Process: 
Use   split   ()   to   help   you   get   the   name   of   the   room   and   the   temperature in the   room on each line   until   you   reach   the   end   of the file.
You will   need to   keep track of when you switch from one room to   the   next, similar to your EMF   implementation.
You will   need a variable to   keep track of how   many   negative readings   in   a row you have read,   and   remember to   reset your   counter when   you start   looking at a   new   room!
Problem 4: Generate a Report 
Submission: You will need to create two new functions in assignment3   .py, get_unique__rooms   ()   and generate_report   ()   as   described   below.   Include   documentation   for   these. You   do not need   to   include   type hints   (e.g., motion   :   list   [str]   or      ->   str), but   you   can   if   you   wish. 
Context: According to this ghost hunting club, you can   identify what   type   of “ghost”   you   are   dealing with   by   looking at combination of evidence; for example, they say that   if   it   is   cold   and there   is   some   electrical interference,   it   must   be a “phantom”   …   I don’t   know.   Either way, a job   is a job.
Helper Function: First, we will   make ourselves a helper function.   A helper function   helps   us   separate   out   a   small   piece of functionality to improve the readability of our code,   even   if   it   is just for a   single function.
Define a function called get_unique__rooms   (motion   ,   emf   ,   temperature)   that accepts three lists of strings and   returns a   list of strings.   It will   look at each   list of rooms   and   return   a   new   list   of all   rooms   that   appeared   in any of the   input lists. This will be   helpful when we are generating   our   report   after.   The   function   can   start   by      making an empty list,looping through each list   of   rooms   passed   as   arguments,   and   appending   the   room   to   the   new combined   list   if it   hasn’t already been   added. 
Generate Report: Define a function called generate_report   (location_name   , motion   , emf   ,   temperature) that will   not return anything.   Motion, emf, and temperature, are   lists   of abnormal   rooms   -   the   ones   that   we   get by calling   read_motion   (),   read_emf   (), and   read_temperature   (). It will compare the rooms in each   list, identify any “ghosts”   based on the   provided criteria, and write these   results   to   a   file. The   file   must   be   named   {location_name}   .report.txt, replacing the location name with the location name that was   passed as   an argument.
Evidence Criteria: 
•    Motion +   EMF + Temperatures   = Poltergeist 
•    Motion   +   EMF   = Oni 
•    Motion + Temperatures   = Banshee 
•    EMF + Temperatures   = Phantom 
On each   line of the   report
Example Result: house.report.txt, extra text not needed
01      == Raven Ghost   Hunting   Society   Haunting   Report ==
02    Location   :   house
03      Found Poltergeist   in   closet
04      Found Oni   in   bathroom
Process: 
Use   your   get_unique__rooms   ()   function   to   get   a   list   of   all   of   the   rooms   that   could   possibly   show   up   in   the             motion,   EMF, or temperature data. Then, cleverly loop through those   rooms   and   check   if the   room   can   be   found   in the different evidence lists.   If it   meets the   criteria, add   the   message   to   the   report,   and   write   that         report to   a file.
NOTE: Your program   must   handle   multiple   runs where we get a   new   report each time. That   is to   say,   you   must either clear the report before appending   to   it,   or write   all   of the   data to   the   report   at   once.
Marking Scheme 
This   marking scheme   is subject to change   if unexpected cases arise   that   need   to   be   addressed   to   meet   the   outcomes discussed   in the specification or if major   requirements are   bypassed.   Execution   marks   can   only   be   provided for code that we can observe running code. We   may   execute   a   different   version   of the   tester that you were provided with which contains additional test cases,   and the   tester   is   provided   as   guidance.
Problem 1 (7 Marks): 
• Execution: Tested   by   running code and observing output
‣   1:   Has   results, and   no duplicates   in   result

‣ 3:   Result contains   only, and   all   of,   correct   outputs
• Approach: Tested   by   reviewing code
‣ 1:   Correctly   Opens/Closes   File
‣ 2: Correctly loops   through   every   line   in   the   file
Problem 2 (10 Marks): 
• Execution: Tested   by   running code and observing output
‣ 1:   Has   results, and   no duplicates   in   result

‣ 6:   Result contains only, and   all   of,   correct   outputs
• Approach: Tested   by   reviewing code
‣   1:   Correctly   Opens/Closes   File

‣ 1:   Correctly   loops through   every   line   in the   file
‣ 1:   Distinguishes   room   names from   readings
Problem 3 (11 Marks): 
• Execution: Tested   by   running code and observing output
‣ 1:   Has   results, and   no duplicates   in   result

‣ 6:   Result contains only, and   all   of,   correct   outputs
• Approach: Tested   by   reviewing code
‣ 1:   Correctly   Opens/Closes   File

‣ 1:   Correctly   loops through   every   line   in the   file
‣ 2:   Function   is well documented
Problem 4 (12 Marks): 
• Execution: Tested   by   running code and observing output
‣ 2: get_unique__rooms   correctly   identifies   rooms   from   all   lists   without   duplicates
‣ 2: Correctly writes to a   new file with   correct filename
‣ 3: Correctly   identifies each   kind of issue without any   false   positives   in   the   report
• Approach: Tested   by   reviewing code   
‣   1:   Correctly   Opens/Closes   File

‣ 2: Does   not   duplicate   logic   intended   for   the   get_unique__rooms   ()   function
‣ 2:   Function   is well documented
Deductions: In addition to standard   packaging deductions, you may   receive deductions   for,   at   minimum,   using   incorrect function   names,   including   print statements   in functions that should not print,   accepting incorrect parameters, incorrect return values, or   other similar   deviations   from   the   specification.
Helpful Tips and Information 
Reminders 
• Element in a list: You can check if a value is   in   a   list   using   the   in   keyword, e.g.,   "a"   in    ["a"   , "b"   , "c"]   is True.
• End of a File: When   a   file   no   longer   has   any   lines   to   read,   readline   ()   will   return   "".
• Lines from a File: readline   ()   will   often   include   spaces   and   newline   characters,   so   using      .strip   ()   can   be very   helpful.
• String Functions: You   will   likely   need   use   of   .strip   ()   and      .split   ()   will   surely   be   helpful   as   well.
A Different File I/O Syntax 
We did   not discuss this   in class, but there   is   a   helpful   alternative syntax   for   opening   files   that   you   are permitted to use and   is generally considered the   “correct” syntax.   This   is   discussed   briefly   in Chapter 11.7 of   the course textbook. 
The Problem: Having to always remember to close an open file   can   lead   to   problems.   While   we   could   blame the   programmer for this   mistake,   in   programming, we usually try to make sure that   important functionality occurs whether somebody makes a mistake   or   not.
The Solution: Context Managers. The specifics of context managers are   not discussed   much   when   learning   Python,   but they are used in a few specific circumstances; using   files   being   one   of the   most   common.
Python   provides   a   special   keyword   structure: with   ..as. Similar   to   how   a   for   loop   abstracts   some   of   the counters away from us to simplify our code and   reduce   errors,   the   with   keyword   hides some   of our open/   close logic.   It is much safer to   use,   because   even   if an   error occurs while working   with   the   file,   the   with      keyword   makes sure to close the file for   us.
Here   is   an   example   of   working   with   a   file   using   with:
01      def   main   ()   :
02          filename =   "my_file   .txt"
03
04          my_text   =   ""
05
06            # Stores the   open   file   reference   as   "f" while   in   this with   block
07            with open   (filename   ,   "r")   as   f   :
08                my_text   =   f   .read   ()
09
10            print(my_text)
Using with   is definitely best practice when working with files and is   encouraged,   but   not   strictly   required.

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
