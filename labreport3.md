# Lab Report 3

**Command 1: find -size**
-

**Example 1**
* The following command searches for and returns all files in `written_2/` that are greater than 100 kilobytes but less than 200 kilobytes. This is useful for finding files that meet a certain size criteria.
```
$ find written_2 -size +100k -size -200k
```

* Output:
```
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/travel_guides/berlitz1/WhereToIndia.txt
written_2/travel_guides/berlitz1/WhereToMalaysia.txt
written_2/travel_guides/berlitz1/WhereToJapan.txt
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
```

**Example 2**
* The following command searches for and returns all files in `written_2/` that are greater than 200 kilobytes. This is useful for finding files that meet a certain size criteria.
```
$ find written_2 -size +200k
```

* Output:
```
written_2/travel_guides/berlitz1/WhereToItaly.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
```

**Source: https://linuxconfig.org/how-to-use-find-command-to-search-for-files-based-on-file-size**

**Command 2: find -type**
-

**Example 1**
* The following command searches for and returns all directories in `written_2/non-fiction/OUP`. This is useful when you only want information on a given path's directories and not the files inside them.
```
$ find written_2/non-fiction/OUP -type d
```

* Output:
```
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Berk
written_2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Rybczynski
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Fletcher
written_2/non-fiction/OUP/Castro
```

**Example 2**
* The following command searches for and returns all files in `written_2/non-fiction/OUP`. This is useful when you only want information on a given path's files and not its directories.
```
$ find written_2/non-fiction/OUP -type f
```

* Output:
```
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written_2/non-fiction/OUP/Abernathy/ch3.txt
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch6.txt
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Abernathy/ch9.txt
written_2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Abernathy/ch14.txt
written_2/non-fiction/OUP/Rybczynski/ch2.txt
written_2/non-fiction/OUP/Rybczynski/ch3.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch3.txt
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch4.txt
written_2/non-fiction/OUP/Kauffman/ch5.txt
written_2/non-fiction/OUP/Kauffman/ch7.txt
written_2/non-fiction/OUP/Kauffman/ch6.txt
written_2/non-fiction/OUP/Kauffman/ch8.txt
written_2/non-fiction/OUP/Kauffman/ch9.txt
written_2/non-fiction/OUP/Kauffman/ch10.txt
written_2/non-fiction/OUP/Fletcher/ch2.txt
written_2/non-fiction/OUP/Fletcher/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch5.txt
written_2/non-fiction/OUP/Fletcher/ch6.txt
written_2/non-fiction/OUP/Fletcher/ch9.txt
written_2/non-fiction/OUP/Fletcher/ch10.txt
written_2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/chQ.txt
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chC.txt
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chV.txt
written_2/non-fiction/OUP/Castro/chW.txt
written_2/non-fiction/OUP/Castro/chM.txt
written_2/non-fiction/OUP/Castro/chZ.txt
written_2/non-fiction/OUP/Castro/chL.txt
written_2/non-fiction/OUP/Castro/chN.txt
written_2/non-fiction/OUP/Castro/chY.txt
written_2/non-fiction/OUP/Castro/chO.txt
```

**Source: https://www.redhat.com/sysadmin/linux-find-command**

**Command 3: find -name**
-

**Example 1**
* The following command searches for and returns `Bahamas-Intro.txt`. This is useful for finding specific files or directories.
```
$ find written_2 -name "Bahamas-Intro.txt"
```

* Output:
```
written_2/travel_guides/berlitz2/Bahamas-Intro.txt
```

**Example 2**
* The following command searches for and returns all files containing `"Bahamas"`. This is useful for finding all files and directories that contain a certain string.
```
$ find written_2 -name "Bahamas*"
```

* Output:
```
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
written_2/travel_guides/berlitz2/Bahamas-Intro.txt
written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt
written_2/travel_guides/berlitz2/Bahamas-History.txt
```

**Source: https://geekflare.com/linux-find-commands/**

**Command 4: find -rm**
-

**Example 1**
