### Syllabus
- Setting up R.
- Data Visualization.
- Parametric Tests.
- ANOVA.
- Non-Parametric Tests.


### What is R?
- A statistical programming language, used for statistical computing and graphical representation.


### R is:
1. A statistical langauge: It is popularly said that **'R is a language made by the statisticians for statisticians'**.
2. A Programming language: Like every other programming language here we have to write codes i.e do programming to derive desired results and accomplish the tasks.
3. An Object Based Language: In R everything we create is saved as an object and all the operations are done on those objects.
4. A Dynamically Typed Language: Unlike programming languages like C, C++, in R there is no need to declare the class of the objects we create. It automatically understands the datatupe of the object.
5. An Open Source Language: It is available to the public and is completely free to use.
6. A Modular Language: There are various libraries (also known as modules) available here which have pre written codes in them and can be used to solve various purposes and expand the capability of the language. It has many packages (libraries of functions) that can be used to solve different problems.
7. It is a great resource for data analysis, data visualization, data science and machine learning.
8. It provides many statistical techniques (such as statistical tests, classification, clustering and data reduction)
9. It is easy to draw graphs in R like pie charts, histograms, box plot, scatter plot, etc.
10. It works on different platforms (Windows, Mac, Linux)
11. It has a large community support

### What can R do?
- We can gain a lot from this language. We can perform a lot of tasks here. Stating a few of them:
1. Descriptive Statistics
2. Inferential Statistics
3. Statistical Modelling
4. Data Visualization
5. Data Manipulation
6. R Programming
7. Machine Learning Modelling
8. Deep Learning Modelling

Next step is the installation of software. Download R and R Studio, alternatively you can install R and R Studio from Anaconda as well.
Get familiar with the R Studio interface majorly with Script, Console, Environment, History, Plots, Packages and Help.
We will be using R Script for this article. To open an R Script just follow these steps.
**R Studio -> File -> New File -> R Script**
Remember: We will be writing the commands/code in the R Script and will look for the output in the Console.

In R Studio we can execute the commands in multiple ways. To execute:
1. A single line of code: Put the cursor on that line and Click on _Run_
2. Multiple lines of code: Select the lines you want to execute and Click on _Run_
3. Entire R file: There are 2 ways for that
    1. Click on Source: This will execute the whole R file and only print the output you want to display.
    2. Click on Source with Echo: This will execute the whole R file but it will print all the commands along with the output you want to display.

Shortcut for the _Run_ button: Ctrl + Enter
Shortcut for the _Source_ button: Ctrl + Shift + S
Shortcut for the _Source with Echo_ button: Ctrl + Shift + Enter

### Syntax Rules in R
- Since the code we write in any programming language consists of logic, function and syntax, it becomes necessary to learn about the R syntax here.

##### Point 1: R is a _case sensitive_ language. Both user defined and predefined objects need to be written as it is.

##### Point 2: Since we talked about the way the objects must be written in R in the above point, it becomes vital to mention some of the rules we need to follow while creating objects in R i.e for the user defined objects. There rules are known as the Object Naming Rules and states that the object name:
1. Can contain only alphabets at the beginning.
2. Can contain both alphabets and numbers.
3. Cannot contain only numbers.
4. Cannot start with a number.
5. Cannot contain any special characters except `.` and `_` which can be included just in between the name and not in the beginning or end.
6. Cannot contain any spaces.
7. Must not coincide with any other object name whether predefined or user defined.