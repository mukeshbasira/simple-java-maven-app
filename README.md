
| PS weekly assignment |
========================

* Page => https://mukeshbasira.github.io/simple-java-maven-app/

1.[WEEK 1](#WEEK-1-BATCH-1)

2.[WEEK 2](#WEEK-2-BATCH-2)

3.[WEEK 3](#WEEK-3-BATCH-1)

4.[WEEK 4](#WEEK-4-BATCH-1)

5.[WEEK 5](#WEEK-5-BATCH-1)

6.[WEEK 6](#WEEK-6-BATCH-1)

7.[WEEK 7](#WEEK-7-BATCH-1)

8.[WEEK 8](#WEEK-8-BATCH-1)

9.[WEEK 9](#WEEK-9-BATCH-1)

10.[WEEK 10](#WEEK-10-BATCH-1)

## WEEK 1 BATCH 1  
link - https://github.com/mukeshbasira/simple-java-maven-app/tree/week1

- Build will be triggered on 12:51 AM everyday( 51 0 * * * (jenkins trigger))

## WEEK 2 BATCH 2
link - https://github.com/mukeshbasira/simple-java-maven-app/tree/week2

![Alt text](UML-Diagrams/UML1.png?raw=true "UML_Diagram_For_DB")

## WEEK 3 BATCH 1
link -  https://github.com/mukeshbasira/simple-java-maven-app/tree/week3


Accept username from user and print prime equivalent of that
example -
 FADE -> d,2,7,b. (hexadecimal equivalent)

## WEEK 4 BATCH 1
link -  https://github.com/mukeshbasira/simple-java-maven-app/tree/week4

Write a java program to accept the string which will give the synonym of the given word, considering below scenario.

1. Initialise a static map with the data structure : Map<String, Set<String>>, which holds the given value

GoodMorning
               { GoodMorning
                Shubhodaya
                Shubhohday
                Bonjour}

GoodEvening
              {  good Evening
                Shubha sange
                susandhya
                Bonsoir}

2. use scanner to accept the string from the end user, assuming if the user gives: GoodMorning, show the values associated for the same.

3. When the user gives GoodBye, which is not there in the Map, ask user if he/she want to add that to the list, when pressed "1", then ask for the synonym in the loop till user enters a empty string, and the given word and synonym to be updated in the map.



## WEEK 5 BATCH 1  
link - https://github.com/mukeshbasira/simple-java-maven-app/tree/week5

Write a java program, to build a quiz application with the below requirements

1. The user should be asked for the question in below format
 
1. who is president of india
a. Donald Trump
b. Ramnath Kovind
c. Narendra Modi
d. None

upon showing the question which is stored in the list (about 10 questions), the user should be allowed to ask the option. 

2. If the user selects correct option show next question failing which a message to be shown "Sorry wrong answer", with the next question.

3. if the user does not answer the question given within 10 seconds then the application to be exited with the message "TIMEOUT!!!"


Helper / Hint:

1. class definition
class Question {
                private String question;
                private String opt1, opt2, opt3, opt4;
                private String correctOpt;
}

2. user daemon threads to tracking
(didn't used threads as of now + Using  TimerTask )
    --- !! working on thread method ---







## WEEK 6 BATCH 1  
link - https://github.com/mukeshbasira/simple-java-maven-app/tree/week6


Question: Consider an application to be developed for various size devices like desktop, tablet, mobile.  And the company wants to test with the POC (Proof Of Concept), below are the requirements.


1. Considering the application is loaded on desktop with size 786*600px the page should load the text with Arial, 36pt, Blue Color.
2. When the page is loaded with 300x350 px then the fonts to be Helvetica, 24pt,, and in Red Color.

3. And when the screen size happens to be 100x100 then font Courier, 18pt, Purple color.



## WEEK 7 BATCH 1  

link - https://github.com/mukeshbasira/simple-java-maven-app/tree/week7


-----Question Topic: Spring Framework IoC------

Question: Consider you are building a Mobile which has dependencies of Camera, Screen, Speaker which has-a relation. 

Below is the prototype of the classes (only sample)
Class -> Mobile
Fields -> camera, speaker, screen



Create .xml files listed below for the classes  
phone.xml  - Mobile
screen.xml – Screen
camera.xml - Camera
speaker.xml – Speaker


Create a App.java file which will load the mobile class

Note: Make sure to use auto wire.


## WEEK 8 BATCH 1  

link - https://github.com/mukeshbasira/simple-java-maven-app/tree/week8

![Alt text](UML-Diagrams/UML2.png?raw=true "UML_Diagram_For_App")

Given the architecture diagram from the manage you are asked to create an end to end program flow with following pointers.

1. The client or CLI is the junit test case you have go have
2. The test cases to be written before the development code to test – with Mockito  - package com.training.mockito
3. Once the development test cases to be written for pass case, fail case and when the business logic throws exception (use custom exception )  - com.training.tests
4. Controller package should take the request and route to service layer  - com.training.controller
5. The service layer will check if the data sent is valid (check if the name of the user is min 4 chars) – then send it to DAO layer  - com.training.service
6. In the DAO layer once the object is got, put a message saying “Record Got Successfully” -com.training.dao
7. Have appropriate contract / interfaces  - com.training.interfaces
8. Keep all exception in – com.training.exceptions


## WEEK 9 BATCH 1

link - https://github.com/mukeshbasira/simple-java-maven-app/tree/week9


![Alt text](UML-Diagrams/UML3.png?raw=true "UML_Diagram_For_Web_App")


Question:

Consider you are asked to create servlets for below end points
/getEmps
/getCustomer
/getProducts

Eventually over course of time the company needs many such servlets due to this maintaining multiple servlets become difficult, create a single servlets which has the signature given below

```xml
<servlet>
                <servlet-name>hi</servlet-name>
                <servlet-class>com.something.ClassName</servlet-class>
</servlet>

<servlet-mapping>
                <servlet-name>hi</servlet-name>
                <url-pattern>/*</url-pattern>
</servlet-mapping>
```


You are asked to create a single servlet which will handle all the scenarios, use either switch case or if condition for routing.



## WEEK 10 BATCH 1

link - https://github.com/mukeshbasira/simple-java-maven-app/tree/week10

Question:

Write a microservice application named

1. meeting-service
2. participant-service

Please keep first set of 5 Meeting in the ArrayList

1. meeting-service

class Meeting 

              {
                
                private int meetingId;

                private String topic;
                
                private String startTime;
                
                private String endTime;
                }

http://localhost:8080/meeting - GET - it should give all the meeting

http://localhost:8080/meeting/1234 - GET - it shoudl give me meeting with id 1234

http://localhost:8080/meeting/1234/participants - GET - get all the participants of meeting id 1234 (from other service)


Please keep first set of 5 Participant in the ArrayList

2. participant-serivce

class Participants 
                   
                   {
                    
                    private int pId;
                    private String pName;
                    private int meetingId;
                    }



http://localhost:8100/participants - GET -- all participants

http://localhost:8100/participant/101 - GET -- participant 101    

Note: Use FEIGN / Rest Template for service communication 
------------------------------------------------------------------------

------------------------------------------------------------------------
