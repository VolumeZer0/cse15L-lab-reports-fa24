# CSE 15L LAB REPORTS SPRING 24

---
## Week 1

1)__cd__
  
  * _no arguments_
  
    __WORKING CLASS DIRECTORY - /Users/khangtran__
    
    ```
    khangtran@Khangs-MacBook-Pro ~ % cd
    khangtran@Khangs-MacBook-Pro ~ % 
    ``` 
    Output? - No output, the program is expecting an input on the next line. failing to provide a valid directory throws an error `zsh:        command not found: akjsdfba`.

    Error? - No, after inputing cd the next line is expecting a directory to be inputed.
  
  * _path to a directory as argument_
  
    __WORKING CLASS DIRECTORY - /Users/khangtran__
    
    ```
    khangtran@Khangs-MacBook-Pro ~ % cd lecture1
    khangtran@Khangs-MacBook-Pro lecture1 % 
    ```
    Output? - No output but it does on the next line what directory it has gone into. By also writting `pwd` it displays a new working         directory (`/Users/khangtran/lecture1`).

    Error? - No, after inputing cd along with a directory as its argument it then proceeds to move into that directory.
  
  * _path to a file as argument_
  
    __WORKING CLASS DIRECTORY - /Users/khangtran/lecture1 __
    
    ```
    khangtran@Khangs-MacBook-Pro lecture1 % cd Hello.java
    cd: not a directory: Hello.java
    khangtran@Khangs-MacBook-Pro lecture1 % 
    ``` 
    Output? - The output tells us that the argument inputed is not a valid directory. By inputting pwd, we can see that our working            directory has not changed.

    Error? - Yes, cd is only meant to move into directories and not files hence why it throws an error when trying to move into a file.

2)__ls__
  
  * _no arguments_
  
    __WORKING CLASS DIRECTORY - /Users/khangtran__
    
    ```
    khangtran@Khangs-MacBook-Pro ~ % ls
    Applications            Desktop                 Library                 Pictures                k.txt                   node_modules            yarn.lock
    Autodesk                Documents               Movies                  Public                  k.txt.pub               package-           lock.json
    Coding                  Downloads               Music                   iCloud Drive (Archive)  lecture1                test.js
    khangtran@Khangs-MacBook-Pro ~ % 
    ``` 
    Output? - by inputting ls, it lists all the files in the current directory.

    Error? - Not an error.
  
  * _path to a directory as argument_
  
    __WORKING CLASS DIRECTORY - /Users/khangtran__
    
    ```
    khangtran@Khangs-MacBook-Pro ~ % ls lecture1 
    Hello.class     Hello.java      README          messages
    khangtran@Khangs-MacBook-Pro ~ % 
    ``` 
    Output? - by inputting ls along with a directory as its argument, it lists all the files in the arguement directory.

    Error? -  Not an error.
  
  * _path to a file as argument_
  
    __WORKING CLASS DIRECTORY - /Users/khangtran/lecture1__
    
    ```
    khangtran@Khangs-MacBook-Pro lecture1 % ls Hello.java
    Hello.java
    khangtran@Khangs-MacBook-Pro lecture1 % 
    ``` 
    Output? - By inputting ls along with a file as its argument, it lists the name of the file as its output.

    Error? - Not an error.

3)__cat__
  
  * _no arguments_
  
    __WORKING CLASS DIRECTORY - /Users/khangtran__
    
    ```
    khangtran@Khangs-MacBook-Pro ~ % cat
    input
    input
    ``` 
    Output? - By inputing cat with no argument, it moves to the next line and prints out what ever is inputed next in a infinite loop.

    Error? - Not an error.
  
  * _path to a directory as argument_
  
    __WORKING CLASS DIRECTORY - /Users/khangtran __
    
    ```
    khangtran@Khangs-MacBook-Pro ~ % cat lecture1 
    cat: lecture1: Is a directory
    khangtran@Khangs-MacBook-Pro ~ % 
    ``` 
    Output? - The output and an error thrown by the program specifying that the input argument is a directory.

    Error? - Yes, cat takes in a file and not a directory hence why an error was thrown.
  
  * _path to a file as argument_
  
    __WORKING CLASS DIRECTORY - /Users/khangtran/lecture1 __
    
    ```
    khangtran@Khangs-MacBook-Pro lecture1 % cat Hello.java
    import java.io.IOException;
    import java.nio.charset.StandardCharsets;
    import java.nio.file.Files;
    import java.nio.file.Path;
    
    public class Hello {
      public static void main(String[] args) throws IOException {
        String content = Files.readString(Path.of(args[0]), StandardCharsets.UTF_8);    
        System.out.println(content);
      }
    }%                                                                                                                                                                              
    khangtran@Khangs-MacBook-Pro lecture1 % 
    ``` 
    Output? - By inputing cat with a file as its argument, it outputs all the text and code in that file.

    Error? - Not an error.
---
