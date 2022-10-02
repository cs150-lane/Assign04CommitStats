# CS150 Assignment 4

File Commit Processing

**Points** : 35

Goals:

1. Read and process data from a file
2. Write C++ code with nested logic
3. Error check your program using multiple test files

We all use GitHub to store our projects, and each time we _push_ to GitHub we create a _commit_. For the purposes of this project, a commit consists of a commit identifier (a string of letter and numbers), a filename, an operation (ADD, DEL, UPD), and the number of lines effected in the file.

You are to write a C++ program that processes the commits from various files and calculates some statistics per file and some summary statistics. The commit information will be maintained in a data file called **commits.txt** with the following format:

commitID0 filename ADD numbLines

commitID1 filename [ADD/DEL/UPD] numbLines

commitID2 fileanme2 ADD numbLines

…

------ 0 END 0

Here is a sample data file:

000001 main.cpp ADD 100

000002 main.cpp DEL 10

a00001 source.cpp ADD 10

a00002 source.cpp ADD 10

a00003 source.cpp UPD 10

------ 0 END 0

**commitID** : these are unique strings of letters and numbers

**filename** : all the operations for one file will be contiguous. Further, the first operation for each file will be ADD.

**ADD/DEL/UPD** : operation performed.

ADD: add lines

DEL delete lines

UPD: update existing lines

**numbLines** : the number of lines affected by the operation.

The last line of the file will always start with six dashes!

The file will always contain correct data with no errors.

There is not keyboard input for this program.

**Your Analysis**

For **each file** you must calculate the following. This must be written to the **screen**.

The initial size: the numbLines given in the first ADD for the file

The ending size: the result of applying the ADD and DEL operations to the initial file size.

The total lines changes: the sum of all the lines changed by any ADD/DEL/UPD operation

The number of commits: how many commits, with any operation, were made on that file.

For **the entire set of commits** you must calculate the following. This must be written to the **screen** :
 File with the most commits: In the event of a tie, list the file which appears earlier in the file.

Average number of lines changed per file: Total lines changed vs total number of files. Display to two digits past the decimal point.

Here is an example of the output after processing the above data file.

Screen output:

\*\*\*\* COMMIT ANALYZER \*\*\*\*

main.cpp

Initial size: 100

Ending size: 90

Total lines changed: 110

Number of commits: 2

source.cpp

Initial size: 10

Ending size: 20

Total lines changed: 30

Number of commits: 3

\*\*\* SUMMARY \*\*\*

File with most commits: source.cpp

Average number of lines changed per file: 70.00

**To complete this assignment you must submit the following:**

1. **An electronic Solution of your program on GitHub**
  1. You are to click on the Assign04 GitHub Assignment Link on Moodle to accept this assignment as we've done in lab. Once accepted, code up a complete solution to the above assignment specification. Your complete solution is to be pushed to GitHub no later than the date and time specified above for your specific section. I will only grade your solution from the proper location on GitHub.
  2. Pay attention to the example output above. Your program's output must look **exactly** like the example output! The spacing and newlines in your output must match exactly.
  3. Make sure that your program compiles and runs correctly with no errors and no warnings. If you get any errors, double check that you typed everything correctly. Be aware that C++ is case-sensitive.
2. **An electronic copy of your program is to be placed on Moodle**
  1. See Lab01 for producing a pdf of your complete program. Once you have produced the pdf of your program and named the pdf your **punetidAssign04** , drop the pdf in the Assign04 folder on Moodle.
  2. The pdf must be in the drop folder on Moodle by the time and day specified above. Anything submitted after that will be considered late.

**NOTES:**

1) You need to edit the data file commits.txt and carefully test your program with many variations of data in the file. After testing, push your final solution using the sample data file listed on the first page.

2) The data file will contain at least one file and the sentinel line.

**IMPORTANT**** :** This is not a last minute assignment. There is a reason you have 12 days to complete this assignment. If you start this assignment the weekend before it's due, there is a high likelihood that you will not finish. Remember also, the tutors are not going to write your code. They will help with a specific issue in your program.

**Good luck! And remember, if you have any problems, come and see straight away.**  ****

5

