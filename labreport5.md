# Lab Report 5

**Lab 6 Grading Script**
-
![image](https://user-images.githubusercontent.com/122562296/224134453-4e86180c-89c3-45f5-81b5-50a0b6c0d26d.png)

**Steps**

* Line 1: Creates the `CPATH` variable containing the command compiling JUnit.
* Line 2: Deletes the `student-submission` directory.
* Lines 3-4: Clones the Git repository specified by the first argument into a new `student-submission` directory.
* Line 5: Prints the message `Finished cloning`.
* Line 7: Changes the current working directory to `student-submission`.
* Lines 8-10, 40-41: Checks if the file `ListExamples.java` exists in the current directory. If it doesn't, prints out the error message `ListExamples.java not found` and exits. If it does, copies `TestListExamples.java` to the `student-submission` directory.
* Lines 12-25, 37-39: Checks to see if the file `ListExamples.class` exists in the current directory. If it doesn't, prints out the error message `Compiler error` and exits. If it does, checks to see if the filter and merge methods are implemented correctly. If they aren't, prints the error message corresponding to the incorrectly implemented method and exits.
* Line 27: Runs the `TestListExamples` tester file and redirects the output to the file `testResults.txt`.
* Lines 29-36: Checks the exit status of the command run in Line 27. If the exit status is `0`, prints the message `All tests have passed`. If the exit status is not `0`, prints out the test results from `testResults.txt` and the error message `One or more tests failed`.
* Line 42-43: Ends the nested if statement and exits the script.
