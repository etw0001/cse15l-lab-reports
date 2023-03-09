# Lab Report 5

**Lab 6 Grading Script**
-
![image](https://user-images.githubusercontent.com/122562296/224136775-6c70c990-b73c-493e-9b59-a4c6c9e035a0.png)

**Steps**

* Line 1: Creates the `CPATH` variable containing the command compiling JUnit.
* Line 3: Deletes the `student-submission` directory.
* Lines 4: Clones the Git repository specified by the first argument into a new `student-submission` directory.
* Line 5: Prints the message `Finished cloning`.
* Line 7: Changes the current working directory to `student-submission`.
* Lines 8-10, 40-41: Checks if the file `ListExamples.java` exists in the current directory. If it doesn't, prints out the error message `ListExamples.java not found` and exits. If it does, copies `TestListExamples.java` to the `student-submission` directory.
* Line 12: Compiles all .java files in the current directory.
* Lines 14-27, 39-41: Checks to see if the file `ListExamples.class` exists in the current directory. If it doesn't, prints out the error message `Compiler error` and exits. If it does, checks to see if the filter and merge methods are implemented correctly. If they aren't, prints the error message corresponding to the incorrectly implemented method and exits.
* Line 29: Runs the `TestListExamples` tester file and redirects the output to the file `testResults.txt`.
* Lines 31-38: Checks the exit status of the command run in Line 27. If the exit status is `0`, prints the message `All tests have passed`. If the exit status is not `0`, prints out the test results from `testResults.txt` and the error message `One or more tests failed`.
* Line 44-45: Ends the nested if statement and exits the script.

**Tested Repositories**

* https://github.com/ucsd-cse15l-f22/list-methods-lab3

![image](https://user-images.githubusercontent.com/122562296/224137439-ab8165b1-0c1f-4592-a604-f455f3c29ca6.png)

* https://github.com/ucsd-cse15l-f22/list-methods-corrected

![image](https://user-images.githubusercontent.com/122562296/224137622-41f5f2b9-e2e6-4357-bbb0-9cdd9eff207f.png)

* https://github.com/ucsd-cse15l-f22/list-methods-compile-error

![image](https://user-images.githubusercontent.com/122562296/224137743-5a4436a0-5ffc-4d02-9e42-ce66483112e4.png)

* https://github.com/ucsd-cse15l-f22/list-methods-signature

![image](https://user-images.githubusercontent.com/122562296/224137858-2d4f723c-adf9-419a-8a7e-d0142a8c918a.png)

* https://github.com/ucsd-cse15l-f22/list-methods-filename

![image](https://user-images.githubusercontent.com/122562296/224137960-ce1b30a7-e0c8-4aed-a750-681bc0b9bae3.png)

* https://github.com/ucsd-cse15l-f22/list-methods-nested

![image](https://user-images.githubusercontent.com/122562296/224138036-279c713d-0299-4444-87af-0e97bbf96534.png)

* https://github.com/ucsd-cse15l-f22/list-examples-subtle

![image](https://user-images.githubusercontent.com/122562296/224138258-f2f99e90-9a74-43ef-8ee7-b8e6ebaea98d.png)
