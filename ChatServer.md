# CSE 15L LAB REPORTS SPRING 24

---
## Week 2/3
---
## Part 1

![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/Screen%20Shot%202024-04-17%20at%206.40.10%20PM.png?raw=true)

---

![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/Screen%20Shot%202024-04-17%20at%206.38.01%20PM.png?raw=true)

_Which methods in your code are called?_ 
In this photo the methods that are called are the handleRequest method in the ServerHandler class.

_What are the relevant arguments to those methods, and the values of any relevant fields of the class?_
The relevant argument in the handleRequest include ' else if (url.getPath().equals("/add-message"))'. This argument to to detect the path to the add-message function. When detected, it takes the quereary and fills in the empty statements with the arguments.

_How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why._
    ```
        String str = "";
        String query = url.getQuery();
        String[] parameters = query.split("&");
        String[] s = parameters[0].split("=");
        String[] user = parameters[1].split("=");
    ```
    
__str__ holds all of the chat history, therefore when the request was made the variable was change to "khang: wassup".

__query__ changes on each request to the users inputed query. In this case "s=wassup&user=khang".

__parameters__ is a list that holds both of the parameters in the query "s" and "user". In this case ["s=wassup", "user=khang"].

__s__ is a list that holds the quaery data for s. In this case ["s", "wassup"].

__user__ is a list that holds the quaery data for user. In this case ["user", "khang"].
    


![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/Screen%20Shot%202024-04-17%20at%206.38.35%20PM.png?raw=true)


_Which methods in your code are called?_ 
In this photo the methods that are called are the handleRequest method in the ServerHandler class.

_What are the relevant arguments to those methods, and the values of any relevant fields of the class?_
The relevant argument in the handleRequest include ' else if (url.getPath().equals("/add-message"))'. This argument to to detect the path to the add-message function. When detected, it takes the quereary and fills in the empty statements with the arguments.

_How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why._
    ```
        String str = "";
        String query = url.getQuery();
        String[] parameters = query.split("&");
        String[] s = parameters[0].split("=");
        String[] user = parameters[1].split("=");
    ```
__str__ holds all of the chat history, therefore when the request was made the variable was change to "khang: wassup evan: niki". 

__query__ changes on each request to the users inputed query. In this case "s=niki&user=evan".

__parameters__ is a list that holds both of the parameters in the query "s" and "user". In this case ["s=niki", "user=evan"].

__s__ is a list that holds the quaery data for s. In this case ["s", "niki"].

__user__ is a list that holds the quaery data for user. In this case ["user", "evan"].


---
## Part 2
---

---
## Part 3
---
In week 2 and 3 I have learned alot of new things including ssh, queries, and paths. ssh allows us to access another computer remotely, and allow people from different computers to connect to one. queries and paths are components of a link that have different affects on the webpage. paths are direct inctructions on where to go from to home page and queries are paramenters inputted into the webstie.


