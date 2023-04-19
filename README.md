# r-basics
In this tutorial we will cover functions, variables, how to import data, and how to run a simple regression
## Functions

  R has all the most common arithmetic functions and follows the standard order of operations (PEMDAS). ``` + ```, ``` - ```, ``` * ```, and ``` / ``` are addition, subtraction, multiplication, and division respectively. There are also some common functions that are very helpful.
```R
  log(1)              # logarithm to base e
## [1] 0
log10(1)            # logarithm to base 10
## [1] 0
exp(1)              # e to the power of
## [1] 2.718282
sqrt(4)             # square root
## [1] 2
2^3                   # 2 to the power of 8
## [1] 8
pi                    # not a function but useful
## [1] 3.141593
```

## Variables/Objects

  To assign a value to a variable all you need to use is the ```<-``` function, the name of the variable you want to create and the value you want to assign to it. It is similar to python in the sense that you do not need to declare the variable's type before assigning it a value. Although ```=``` can also be used to assign values to variables it is typically considered bad practice since it can only be used at the top level (e.g., in the complete expression typed at the command prompt) or as one of the subexpressions in a braced list of expressions(ex: ). On the other hand, ```->``` can be used anywhere and has an unambigous meaning.
```R
  x <- 1              #assigns the variable x with the value 1
  y <- "Apple"        #assigns variable y with the Characters "Apple"
  3 -> z              #rightward assignment
  
  x
## [1] 1
  y
## [1] Apple
  z
## [1] 3
```
  Now that we know how to write functions, what if we want to assign these to a variable. It is important to recognize that R is an object oriented programming and has several fundamental primitive types that you can work with. R has five basic object types: integers, doubles, booleans, characters, complex, and raw binary.
  Integers are denoted with an "L" following the variable. They have no decimal component and aren't as commonly used as doubles which do include decimals and are more straightforward to declare(in our previous example x and z are doubles). Booleans are denoted using the reserved words ```TRUE``` and ```FALSE```. Characters are what a more traditional programming student would think of as strings
