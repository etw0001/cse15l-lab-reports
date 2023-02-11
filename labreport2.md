# Lab Report 2

**Part 1**
-

**Below is the code for my `StringServer`:**

![image](https://user-images.githubusercontent.com/122562296/215363739-993e6d2a-2b3e-4aef-a5a7-61336adc0a97.png)

**First iteration of `/add-message`:**

![image](https://user-images.githubusercontent.com/122562296/215364827-fc7270fb-099d-4403-abd0-571e1153b0ea.png)

* In the first iteration of `/add-message` (shown above), the method `handleRequest` is called. `handleRequest` calls `getPath` and `getQuery` to determine the path and query of the URL, respectively. To check that the URL contains "/add-message", the `contains` method is called, taking in "/add-message" as a string argument. Next, `handleRequest` calls `split`. This method takes in "=" as a string argument and splits the query string into an array, using "=" to separate the parameters. The `equals` method takes in "s" as a string argument to verify that the first element of the array is equal to "s". After this is confirmed, `handleRequest` appends the value of the query string after the equals sign to `str`.
* The argument passed into `handleRequest` is `url`, an object of type `URI`. `str` is the string in which the value after the equals sign in the URL (Ethan) will be concatenated to, followed by a newline character.

**Second iteration of `/add-message`:**

![image](https://user-images.githubusercontent.com/122562296/215364860-5a4375f6-9400-468c-9a9a-33b45f7f781e.png)

* In the second iteration of `/add-message` (shown above), the method `handleRequest` is called.
* The argument passed into `handleRequest` is `url`, an object of type `URI`. `str` is the string which the value after the equals sign in the URL (CSE15L) will be concatenated to in a new line. Due to this, str becomes a multiline string, containing "Ethan" in the first line and "CSE15L" in the second.

**Part 2**
-

**The buggy `reverseInPlace` method in `ArrayExamples.java` had inputs that both did and didn't induce failure.**

**Below is an example of an input that induces failure:**
```
  @Test
  public void testReverseInPlace() {
    int[] input1 = {1, 2, 3};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{3, 2, 1}, input1);
  }
```

**Below is an example of an input that doesn't induce failure:**
```
  @Test
  public void testReverseInPlace2() {
    int[] input1 = {3, 2, 3};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{3, 2, 3}, input1);
  }
```

**Below are the symptoms of running the tests shown above:**

![image](https://user-images.githubusercontent.com/122562296/215377731-ea4bfc24-9899-4702-90d9-06f8ce014e46.png)
![image](https://user-images.githubusercontent.com/122562296/215377849-a8c1d2f4-d4ec-4b57-91b0-35b8413abd5d.png)

**Shown below is the code before and after fixing the bug:**

**Before:**
```
  static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```
**After:**
```
  static void reverseInPlace(int[] arr) {
    int[] tempArr = new int[arr.length];
    for(int i = 0; i < arr.length; i++)
      tempArr[i] = arr[arr.length - i - 1];

    for (int i = 0; i < arr.length; i++)
      arr[i] = tempArr[i];
  }
```

* The fix adds a temporary array for the elements to be copied onto so that they can all be properly transferred.

**Part 3**
-

**Something I learned from lab over the last 2 weeks was how to build a web server that takes in a URL as an input and displays text on a web page as an output. I also learned how to run the server both locally and remotely.**
