### CTIS 210 Project 6

This project will build familiarity with constructing a full Java program. This first program will be simple and based on what you did for Project 5. And you must have Project 5 completed before beginning this project. You should have your Project 5 notebook open in a separate window as you work on this project. 

This project has a file RegistrationPoints.java that includes a `main` method. You will do all your work for this project in this file. Your goal is to produce a program that does all the same work as the Project 5 notebook, but in a standard Java application file. The result should be a program that generates 18,357 random students, calculates their registration points, and creates a histogram of that information.

In RegistrationPoints.java, you will see several comments that guide where specified statements and methods should be placed. The following instructions will help as well. (If you are feeling comfortable with how a Java program should be constructed, you might try building the program on your own.)

During this process, if you get any errors that you are not sure how to fix or you are having any other problems, then commit and sync your project, and email the instructor.

Note that you will not be told to run the program until it's specified after a few tasks. While you should be able to run the program at the end of each task without any errors, you also won't see any output displayed until that point where you're explicitly directed to run the program.

#### Methods task

In project 5, there is a magic code cell with two methods definitions: `calculateTotalCredits` and `calculatePoints`. Copy the code in that cell and paste it in the designated place in RegistrationPoints.java. 

You'll need to make one change: Add the keyword `static` so that each signature starts with `public static double`. We're not ready yet to describe why that's necessary. But in general, methods in the file with the `main` method need have `static` in their signature.

Don't continue to the next task if there are any errors present.


#### Functionality import task

This program will use the `Random` and `Arrays` classes that Java makes available. We use `import` statements to tell Java that we intend to use those classes in this program. 

Add the following lines to the place in the program that specifies where import statements go.

```java
import java.util.Arrays;
import java.util.Random;
```

#### Array declaration task

The final Project 5 notebook includes declaration of arrays that contain the data necessary to calculate registration points. 

Declare those same arrays in the specified location in RegistrationPoints.java.

#### Array assignment, point calculation, and histogram task

At this point, we have all the framework we need to make the program do something. We're going to focus just on the work with the arrays. Add the statements from Project 5 in the specified place that

* Use one or more loops to fill the arrays with random values
* Calculate the registration points for each student
* Summarize the data using histograms
* Display the histogram using the `Arrays.toString()` method

Once you have added these statements, run the program. You should then see output displayed in the terminal that looks similar to what you saw in Project 5. 

#### Improving program maintenance task 

At this point, you should have a fully working Java program that achieves the same goals as Project 5. But there's a flaw that makes the program less flexible. In the program, you should see multiple places where 18357 is used as the number of students. If we want to change the number of students, we have to change that in all those places, which can lead to errors. 

Instead, we should declare a variable for the number of students, initialize it with the value 18357, and then use that variable wherever the number of students is being referred to.

Your task is to do exactly that: Declare the variable and assign it with its initial value. Use that variable any place the value 18357 is currently used. Show that the program still works as it should when you change the value it's initialized with.

#### Submitting your assignment

Make sure all files are saved. Commit and sync the project as you've done with other project. You do not need to close an issue.

You should go into the Project 6 assignment in Canvas and just submit the text "My Project 6 is now ready for evaluation". That indicates that your project on GitHub is complete.

#### Optional challenge exercises

* Add in any of the challenge exercises from Project 5 to this program.
* Instead of initializing the number of students in the program, prompt the user for that number of students when the program starts and use that value.
* Adjust the program so that the user can choose the number of bins in the histogram.