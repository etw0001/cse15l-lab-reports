# Lab Report 4

**Logging into ieng6**
-
**Keys pressed:**

`<^R> ssh <enter>`
* I accessed the command `ssh cs15lwi23agb@ieng6.ucsd.edu` using `<^R>` to search for a command containing "ssh" in my command history, then pressed `<enter>` to run it. This connected me to the `ieng6` remote server.

**Cloning my fork of the repository from my GitHub account**
-
**Keys pressed:**

`<^R> clone <enter>`
* I accessed the command `git clone git@github.com:etw0001/lab7.git` using `<^R>` to search for a command containing "clone" in my command history, then pressed `<enter>` to run it. This cloned my fork of the `lab7` repository from my GitHub account.

**Running the tests and demonstrating that they fail**
-
**Keys pressed:**

`cd lab7`
* I used `cd` to set my current working directory to `lab7`.

`<^R> * <enter>`
* I accessed the command `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` using `<^R>` to search for a command containing "*" in my command history, then pressed `<enter>` to run it. This compiled the testers.

`<^R> List <enter>`
* I accessed the command `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` using `<^R>` to search for a command containing "List" in my command history, then pressed `<enter>` to run it. This ran the testers.

**Editing the code file to fix the failing test**
-
**Keys pressed:**

`<^R> nano <enter>`
* I accessed the command `nano ListExamples.java` using `<^R>` to search for a command containing "nano" in my command history, then pressed `<enter>` to run it. This opened the `nano` editor and loaded the contents of `ListExamples.java`.

`<right> <right> <right> <right> <right> <right> <right> <right> <right> <right> <right> <right> <delete> 2`
* I used the scroll wheel to move the cursor from the 1st line of the code file to the 43rd line, pressed `<right>` 12 times to move the cursor rightward to the location where I wanted to make changes, then pressed `<delete>`, followed by `2`, to change `index1` to `index2`.

`<^O> <enter> <^X>`
* I pressed `<^O> <enter>` to save/overwrite `ListExamples.java` then pressed `<^X>` to exit the editor.

**Running the tests and demonstrating that they now succeed**
-
**Keys pressed:**

`<^R> * <enter>`
* I accessed the command `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` using `<^R>` to search for a command containing "*" in my command history, then pressed `<enter>` to run it. This recompiled the testers.

`<^R> List <enter>`
* I accessed the command `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` using `<^R>` to search for a command containing "List" in my command history, then pressed `<enter>` to run it. This reran the testers.

**Committing and pushing the resulting change to my GitHub account**
-
**Keys pressed:**

`git add L <tab> .j <tab>`
* I accessed the command `git add ListExamples.java` quicker by using `<tab>` to autofill parts of my command twice. This staged the changes for the next commit.

`git commit -m "updated"`
* This created a new commit that included those changes.

`git push`
* This pushed the changes I made on my local repository to my GitHub repository.

**Sources used**
-
**ChatGPT**
