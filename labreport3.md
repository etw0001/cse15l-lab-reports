# Lab Report 3

**Command 1: find -size**
-

**Example 1**
* The following command searches for and returns files in `written_2/` that are greater than 100 kilobytes but less than 200 kilobytes. This is useful for finding files that meet a certain size criteria.
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
* The following command searches for and returns files in `written_2/` that are greater than 200 kilobytes. This is useful for finding files that meet a certain size criteria.
```
$ find written_2 -size +200k
```

* Output:
```
written_2/travel_guides/berlitz1/WhereToItaly.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
```
