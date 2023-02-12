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
* The following command searches for and returns all directories in `written_2/`. This is useful when you only want information on a given path's directories and not the files inside them.
```
$ find written_2 -type d
```

* Output:
```
written_2
written_2/non-fiction
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Berk
written_2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Rybczynski
written_2/non-fiction/OUP/Kauffman
written_2/non-fiction/OUP/Fletcher
written_2/non-fiction/OUP/Castro
written_2/travel_guides
written_2/travel_guides/berlitz1
written_2/travel_guides/berlitz2
```

**Example 2**
* The following command searches for and returns all files in `written_2/`. This is useful when you only want information on a given path's files and not its directories.
```
$ find written_2 -type f
```

* Output:
```
All files in the `written_2/` directory (not shown due to size)
```

**Source: https://www.redhat.com/sysadmin/linux-find-command**

**Command 3: find -**
-

**Example 1**
* oki
