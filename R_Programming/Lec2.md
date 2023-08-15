### Writing comments in R
- Single line comment: Use the `#` symbol at the beginning of the line. This symbol can be placed anywhere in the line and everything following the symbol gets commented i.e is not executed
- Multiple line comments: To comment a set of lines i.e make them unexecutable, select those lines and press Ctrl + Shift + C.

We can write multiple commands in a single line just by separating the different commands with the `;` operator.

How? for the following code:
var1=100

```
> var1=100
> var2=200
> var3=var2-var1
> var3
[1] 100
> var1=100;var2=200;var3=var2-var1
> var3
[1] 100
```

### Operators in R
- Arithmetic Operators: `+`,`-`,`*`,`/` (gives exact answer), `%%` (the modulus operator which gives the remainder), `%/%` (results in integer division)
- Relational Operators: `=`,`==`,`!=` results in the output are TRUE or FALSE
- Logical Operators: `&` (and), `|` (or)
- Assignment Operators: `=`, `<-`,`->` `<-` is going to be the most used operator while writing R commands where as `->` is going to be the least used.
    - What about `=`? You must have encountered that `=` is used as an assignment operator in most of the other tools that we have including Python.
    - Well, in R both `=` and `<-` can be used to assign values however they do differ in some sense which you will get to know when you learn about data manipulation in R.

### Data Types in R
1. Text: This category can further be classified into _character_ and _factor_. If anything is stored in `""` or `''` it has a class of character.
2. Number: This category can further be classified into _numeric_, _integer_ and _complex_. However, we will be encountering the _numeric_ type the most in this case.
3. Boolean: We have _logical_ data type here which is apparently for the TRUE and FALSE output we receive.
4. Date: The most complicated data type in R, it is not a direct data type but instead a derived data type and hence a whole new topic which needs to be discussed separately.

Essentially, Type Casting is the process of changing the data type of an object in R to another data type.
Suppose we have an object `"demo"` with us having any particular data type. To see this object in the form of another data type say "new_datatype" we write the command as `as.new_datatype(demo)` and we are done.


Similarly, we can write commands like:
```
as.character(demo)
as.numeric(demo)
as.logical(demo)
as.integer(demo)
```
and so on....

But this process has some rules, not every datatype can be transferred to another type. There is a precedence that these data types follow according to which type casting is done. Taking the most used data types: character, numeric, logical.
In general, for any object the class cannot be converted from character to numeric to logical. Similarly for any object the class cannot be converted from numeric to logical.

### Libraries in R
- We touched on this part at the beginning when we discussed that R is a modular language and therefore has something known as a **library** (also called module). R has two kinds of libraries: System libraries and User libraries which are more than 18,000 in number.
- These libraries are available on **CRAN** (Comprehensive R Archive Network) which is global repository of open-source packages.
- Now when it comes to libraries in R there are 3 things to keep in mind: Available libraries, Installed libraries and Loaded libraries.
- While available libraries refer to all packages there on CRAN, installed libraries refer to all those libraries which are installed in your system and the loaded libraries are the ones that you explicitly load each time you open R in order to use the various functions listed there.

##### How to install a library?
- Go to Packages -> Install -> Give the Package Name

##### How to Load a library?
- Having a library installed in your system doesn't mean that you can use it (functions defined inside) any time rather you need to explicitly load the library and the preferred way of doing the same is: `library(library_name)`
(Note: **dplyr** is one of the most commonly used libraries in R which contains various important functions (predefined functions) in it used for the purpose of data manipulation in R. Some of the commonly used functions defined in dplyr are `mutate()`, `rename()`, `filter()`, etc.)
- The operator `::` denotes that we are referring to the mutate function from the dplyr library

```
> "Hello World!"
[1] "Hello World!"
> 5+5
[1] 10
> plot(1:10)
> print("Hello World!")
[1] "Hello World!"
> for (x in 1:10)
+ {
+ print(x)
+ }
[1] 1
[1] 2
[1] 3
[1] 4
[1] 5
[1] 6
[1] 7
[1] 8
[1] 9
[1] 10
```

### R Comments

```
> Hello World!
Error: unexpected symbol in "Hello World"
> # Hello World!
> #Hello World!
```

### R Variables
```
> name <- "John"
> age <- 40
> print(name)
[1] "John"
> print(age)
[1] 40
```

### Concatenate
```
> text <- "awesome"
> paste("R is",text)
[1] "R is awesome"
> txt1 <- "R is"
> txt2 <- "awesome"
> paste(txt1,txt2)
[1] "R is awesome"
```

------


```
> num1<-5
> num2<-10
> num1+num2
[1] 15
```

```
> txt1+num2
Error in txt1 + num2 : non-numeric argument to binary operator
```

```
> var1<-var2<-var3<-"Orange"
> var2
[1] "Orange"
> var1
[1] "Orange"
> var3
[1] "Orange"
```

#### Legal variable names
```
> myvar<-"John"
> my_var<-
+ "John"
> myVar<-"John"
> MYVAR<-"John"
> myvar2<-"John"
> .myvar<-"John"
> myvar
[1] "John"
> my_var
[1] "John"
> myVar
[1] "John"
> MYVAR
[1] "John"
> myvar2
[1] "John"
> .myvar
[1] "John"
```

#### Illegal variable names
```
> 2myvar<-"John"
Error: unexpected symbol in "2myvar"
> my-var<-"John"
Error: object 'my' not found
> my var<-"John"
Error: unexpected symbol in "my var"
> _my_var<-"John"
Error: unexpected symbol in "_my_var"
> my_v@ar<-"John"
Error: object 'my_v' not found
> TRUE <- "John"
Error in TRUE <- "John" : invalid (do_set) left-hand side to assignment
```