# Debug-Python-Code

<h2>Introduction</h2>

One of the biggest challenges faced by analysts is ensuring that automated processes run smoothly. Debugging is an important practice that security analysts incorporate in their work to identify errors in code and resolve them so that the code achieves the desired outcome.

Through a series of tasks in this lab, I'll develop and apply my debugging skills in Python.

<h2>Scenario</h2>

In my work as a security analyst, I need to apply debugging strategies to ensure my code works properly.

Throughout this lab, I'll work with code that is similar to what I've written before, but now it has some errors that need to be fixed. I'll need to read code cells, run them, identify the errors, and adjust the code to resolve the errors.

<h2>Task 1</h2>

The following code cell contains a syntax error. In this task, I'll run the code, identify why the error is occurring, and modify the code to resolve it. (To ensure that it has been resolved, run the code again to check if it now functions properly.)

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/1e5dd6a1-d814-4e84-b430-1a1f273c8f32)

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/e8017c89-7e98-446b-b9d0-31021cd74f2c)

When the code is run before it's modified, the output shows SyntaxError: invalid syntax, which indicates that there is a syntax error. The syntax error is caused by the missing ```:``` at the end of the for loop header. To fix this, I can add ```:``` at that position.

<h2>Task 2</h2>

In the following code cell, I'm provided a list of usernames. There is an issue with the syntax. In this task, I'll run the cell, observe what happens, and modify the code to fix the issue.

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/2ae8c664-6751-4fb6-b9b8-d572985cb456)

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/06c7044b-e7bc-4b46-a64e-fb008a5b665b)

When the code is run before it's modified, the output shows SyntaxError: invalid syntax. The issue occurred when assigning a value to usernames_list. The fourth username is missing a closing quotation mark, and there is a missing comma between the fourth and fifth usernames. Each username in the list should be a string, and commas should be used to separate one username from the next. To fix the syntax error, I can add a closing quotation mark to properly specify the fourth username as a string and then add a comma between the fourth and fifth usernames to separate them. So instead of ```"zdutchma "esmith",```, it should say ```"zdutchma", "esmith",```.

<h2>Task 3</h2>

In the following code cell, there is a syntax error. My task is to run the cell, identify what is causing the error, and fix it.

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/23cdb5e3-36e0-4a19-8cd0-f5e22367ef50)

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/c073fc10-a3ff-4400-bbd9-8543c3b01496)

When the code is run before it's modified, the output shows SyntaxError: unexpected EOF while parsing. This is caused by the missing closing parenthesis at the end of the print() statement. To fix this, I can add ```)``` at the end of the line.

<h2>Task 4</h2>

In the following code cell, I'm provided a usernames_list, a username, and code that determines whether the username is approved. There are two syntax errors and one exception. My task is to find them and fix the code. A helpful debugging strategy is to focus on one error at a time and run the code after fixing each one.

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/fe70ba2c-2263-43e5-8adc-b82f60eba16f)

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/f241db71-251d-4efb-b540-cde9e6185be3)

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/e4c883ab-88fa-4df5-a18c-1b38955adabd)

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/f55b9606-90a5-43ac-83e0-50252a27106d)

When the code is run before it's modified, the output shows SyntaxError: invalid syntax, as that's the first error that Python encounters in this code. There are three issues in the code:

1. In the if condition, the ```=``` assignment operator is used instead of the == comparison operator, causing a syntax error. To fix this, I can replace ```=``` with ```==```.
2. Inside the if statement, indentation is missing, causing a syntax error. To fix this, I can add an appropriate indentation before the print() statement.
3. The variable usernames_list is misspelled in the for loop condition. It's spelled as username_list there, causing an exception. To fix this, I can add the missing s in the appropriate spot.

<h2>Task 5</h2>

In this task, I'll examine the following code and identify the type of error that occurs. Then, I'll adjust the code to fix the error.

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/a93cb9f6-850f-4dcd-b762-302a52bbd762)

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/3ccdd6a9-48d2-4a14-9c56-7ded7404989b)

When the code is run before it's modified, the output shows IndexError: list index out of range, which means that there is an index error, and it's caused by an invalid index value that is being used with a list. Note that an index error is a type of exception in Python. Also, recall that indexing in Python starts at 0 and the usernames_list has a length of 5. So 4 is the index value that corresponds to the final element in usernames_list. 5 is not a valid index in usernames_list. I can fix the error by replacing 5 with 4.

<h2>Task 6</h2>

In this task, I'll examine the following code. The code imports a text file into Python, reads its contents, and stores the contents as a list in a variable named ip_addresses. It then removes elements from ip_addresses if they are in remove_list. There are two errors in the code: first a syntax error and then an exception related to a string method. My goal is to find these errors and fix them.

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/3048a336-183d-4279-b884-88039f2b3148)

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/179b14cd-fea2-43a8-8a0d-a2d4a312839e)

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/a54e39a6-5c2c-47d5-bfba-a749292088cf)

When the code is run before it's modified, the output shows SyntaxError: invalid syntax, as that's the first error that Python encounters in this code. There are two errors in the code:

1. There is a syntax error because the header of the with statement is missing a ```:``` at the end. To fix this, I can add ```:``` there.
2. There is an exception related to the string method .split(). To call this method, I must write the name of the variable that contains the string you want to use, followed by a ., and then the name of the method. So to fix this, I can replace split.ip_addresses() with ip_addresses.split().

<h2>Task 7</h2>

In this final task, there are three operating systems: OS 1, OS 2, and OS 3. Each operating system needs a security patch by a specific date. The patch date for OS 1 is "March 1st", the patch date for OS 2 is "April 1st", and the patch date for OS 3 is "May 1st".

The following code stores one of these operating systems in a variable named system. Then, it uses conditionals to output the patch date for this operating system.

However, this code has logic errors. My goal is to assign the system variable to different values, run the code to examine the output, identify the error, and fix it.

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/aff2002e-0879-4350-a7e6-dcee71671041)

![image](https://github.com/n8som/Debug-Python-Code/assets/110139109/fde11ab7-1683-4c5d-a170-6cfa0bb80b90)

When the code is run before it's modified, the system variable is assigned to "OS 2", but the output is Patch date: March 1st. This is not the correct patch date for OS 2.

When assigning the system to "OS 1", the output is Patch date: May 1st. This is not the correct patch date for OS 1.

These logic errors are due to the incorrect index values in the first and second print() statements in the code. Note that indexing in Python starts at 0 and patch_schedule is in order of operating system from OS 1 to OS 3. To fix the logic errors, I can use patch_schedule[0] to get the correct patch date for OS 1 and patch_schedule[1] to get the correct patch date for OS 2.

<h2>Conclusion</h2>

What are the key takeaways from this lab?

- Debugging is an essential practice that analysts use to identify errors in code and fix them to ensure that the code runs smoothly.
- Python executes code from top to bottom and stops once it encounters an error. So if there are multiple errors in a code cell, the outputted error message will typically show the first error.
- In Python, common types of errors include syntax errors, logic errors, and exceptions.
  - Syntax errors often involve punctuation such as a missing ```:``` at the end of a ```with``` statement header and a missing ```,``` between elements in a list.
  - Logic errors could involve incorrect indices when accessing elements from a list.
  - Exceptions could involve misspelled variable names or incorrectly called string methods.
- A key strategy for debugging is running code and examining if it produces the intended results. If the output isn't correct, or if it displays an error message, use this to identify which line(s) of the code could be causing the issue. After fixing the code, it's important to run it again to ensure that everything works as expected.
