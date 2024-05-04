# CSE 15L LAB REPORTS SPRING 24

---
## Week 5
---
## Part 1 - Bugs
---

1.A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown).
  ```
    @Test
    public void testReverseInPlace2(){
      int[] intArr = {1, 2, 3, 4 };
      ArrayExamples.reverseInPlace(intArr);
      assertArrayEquals(new int[]{4, 3, 2, 1}, intArr);
    }
  
    @Test
    public void testReversed2(){
      int[] intArr = {5, 3, 0, 0, 5 };
      assertArrayEquals(new int[]{5, 0, 0, 3, 5 }, ArrayExamples.reversed(intArr));
    }

  ```
2.An input that doesn't induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown).
  ```
      @Test
      public void testReverseInPlace2(){
        int[] intArr = {1, 2, 3, 4};
        ArrayExamples.reverseInPlace(intArr);
        assertArrayEquals(new int[]{4, 3, 3, 4}, intArr);
      }
    
      @Test
      public void testReversed2(){
        int[] intArr = {1, 2, 3, 4};
        assertArrayEquals(new int[]{4, 3, 3, 4}, ArrayExamples.reversed(intArr));
      }
    
  ```
3.The symptom, as the output of running the two tests above (provide it as a screenshot -- one test should pass, one test should fail).

![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/Screen%20Shot%202024-05-04%20at%201.12.07%20AM.png?raw=true)

4.The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown).

Before:
  ```
    // Changes the input array to be in reversed order
    static void reverseInPlace(int[] arr) {
      for(int i = 0; i < arr.length; i += 1) {
        arr[i] = arr[arr.length - i - 1];
      }
    }
  
    // Returns a *new* array with all the elements of the input array in reversed
    // order
    static int[] reversed(int[] arr) {
      int[] newArray = new int[arr.length];
      for(int i = 0; i < arr.length; i += 1) {
        arr[i] = newArray[arr.length - i - 1];
      }
      return arr;
    }
  ```
After:
  ```
    // Changes the input array to be in reversed order
    static void reverseInPlace(int[] arr) {
      int[] newArray = new int[arr.length];
      for(int i = 0; i < arr.length; i += 1) {
        newArray[i] = arr[arr.length - i - 1];//CHANGES: added a temp arr in order to have the items at the end copied
      }
      for(int i = 0; i < arr.length; i++){
        arr[i] = newArray[i];
      }
    }
  
    // Returns a *new* array with all the elements of the input array in reversed
    // order
    static int[] reversed(int[] arr) {
      int[] newArray = new int[arr.length];
      for(int i = 0; i < arr.length; i += 1) {
        newArray[i] = arr[arr.length - i - 1];//CHANGES: same change
      }
      return newArray;//changed from arr to newArry
    }
  ```
5.Briefly describe (2-3 sentences) why the fix addresses the issue.

  The fix addresses the issue because because it reverses the array in a output array instead of in the inputted one. This way when the values are being coppied over in reverse   order, the values that are in the begining are copied over aswell.

---
## Part 2 - Researching Commands
---
  __Examples:__
    
  _grep:_
    __Ex 1:__
      __Input:__
        ```
          grep -c ".txt" find-results.txt 
        ```
      __Output:__
        ```
          1391
        ```
      Explanation:
      -c is a option avalible to the grep command that instead returns the count of the occurances of the matching pattern. This is usefull in the case that you only want the count of how many and not the files themselves.
    
    __Ex 2:__
      __Input:__
        ```
          grep -v ".txt" find-results.txt
        ```
      __Output:__
        ```
        technical
        technical/government
        technical/government/About_LSC
        technical/government/Env_Prot_Agen
        technical/government/Alcohol_Problems
        technical/government/Gen_Account_Office
        technical/government/Post_Rate_Comm
        technical/government/Media
        technical/plos
        technical/biomed
        technical/911report
        ```
      __Explanation:__
      -v is an option avalible to the grep command. This option makes it so that the command prints the commands that do not match the pattern instead of printing the files that do. This is useful when you want to exclude a certain file type or name but not any other.
    
  _less:_
    Ex 1:
    Input:
    Output:
    Explanation:
    Ex 2:
    Input:
    Output:
    Explanation:
    
  _find:_
    Ex 1:
    Input:
    Output:
    Explanation:
    Ex 2:
    Input:
    Output:
    Explanation:
    
  __Citations__
  * [grep resources][https://www.geeksforgeeks.org/grep-command-in-unixlinux/]
  * [find resources][https://www.geeksforgeeks.org/find-command-in-linux-with-examples/#options-available-in-find-command-in-linux]
  * [less resources][https://www.geeksforgeeks.org/less-command-linux-examples/]


