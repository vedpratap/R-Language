# R-Language
Personal Note

## What is RStudio ?
- It is a free, open source integrated environment or IDE for R (the statistical programming language).
- RStudio helps to keep R more organized and it adds more functionality to it.

```
 > x<-1:5        //Will create vector x having value 1 to 6 i.e 1 2 3 4 5
 > y<-6:10       //Will create vector y having value 1 to 6 i.e 6 7 8 9 10
 > plot(x,y)     //Will plot graph between x & y
 > ls()          //list all the variables in working memory.
```
- If we are using simple R console then we can export plots as a picture but with less functionality in comparison to RStudio (Using `Export`).

## Importing data in RStudio

- `Environment` - `Import Dataset` - `from local file` - `select Dataset` - `import` (We can modify while importing also)

## Create and Manage scripts in RStudio

- `File` - `New File` - `R Scripts`
- Write some codes inside it and `Run` it.
- It will get executed inside `R` Console.
- `> sum(x,y,z)  //Will add all the numbers of all the variables/vectors`
- `File` - `New File` - `R Markdown` : It allows you to embed R code and R output directly into documents, pdf, HTML, Word, etc..
-  `File` - `New Project..` : It allows you to manage all your files and output related to a project in one spot!

## How to install R and RStudio ?
- https://teacherscollege.screenstepslive.com/a/1108074-install-r-and-r-studio-for-windows

## Getting started with R_Basic Arithmetic and Coding in R

```
> x = 11       // Assigning value to a variable/object (It is case sensitive)
> print(x)     // Printing value of x.
> x            // We can also print value by writing only object name.

> x <- 11      // Another way to assigning value. We can use anyone because it is just a matter of preference. "<-" is better choice than "="

> x <- 45      // R usually override the object value. i.e now value of x is 45 in workspace memory also.

> rm(x)        // rm() - used to remove object i.e x from workspace memory.

```
- Object names are `case sensitive` : object `MyObject` is not the same as `myobject`
- They can contains both `numbers` or `letters` but should `START` with a letter, e.g. `2myobject` is not a valid
- You can use `underscores`. Other `special characters` should be avoided.
- Avoid using `function names` as object names.

```
> xx <- "ved"    // Assigning string
> yy <- "1"      // Assigning number as string
> 11+19          // Arithmetic oper. on number
> 11*19
> x+y            //  // Arithmetic oper. on objects
> x-y
> x/y
> x*y
> y^2            // ^ - to the power
> y^2 + x^2
> sqrt(y)
> y^(1/2)
> log(y)         // To base 10
> exp(y)
> log2(y)        // To base 2
> abs(-14)

>  # comments will be here....  // Comments will start with '#'
```

- If we write incomplete command in console it will replace `<` to `+`. But after writing remaining command and press enter it will return back to `<`
- We can use `arrow keys` on keyboard to move amongs written commands.

## Create and Work with Vectors and Matrices in R

```
> x1 <- c(1,3,5)                                                 // Vector x i.e 1 3 5
> gender <- c("male", "female")                                  // Vector gender i.e male female
> 2:7                                                            // 2 3 4 5 6 7
> seq(from=1, to=7, by=1)                                        // 1 to 7 (inclusive) increment by 1
> seq(from=1, to=7, by=1/3)                                      // 1 to 7 (inclusive) increment by 1/3
> seq(from=1, to=7, by=0.25)                                     // 1 to 7 (inclusive) increment by 0.25
> rep(1, times=10)                                               // repeat 1 10 times i.e 1 1 1 1 1 1 1 1 1 1
> rep("ved", times=5)                                            // ved ved ved ved ved
> rep(1:3, times=4)                                              // 1 2 3 1 2 3 1 2 3 1 2 3
> rep(seq(from=1, to=7, by=0.25), times=2)                       // repeat the whole seq. 2 times
> rep(c(1,3,5), times=3)                                         // 1 3 5 1 3 5 1 3 5
> x <- 1:5                                                       // assigning value to object i.e x 1 2 3 4 5
> y <- c(1,5,3,4,8)                                              // y is a vector
> x+10                                                           // add 10 to all the elements of a vector or sequence
> x*10                                                           // multiply 10 to all the elements of a vector or sequence
> x/2                                                            // divide by 10 to all the elements of a vector or sequence
>
> # If the length of two vector are same, we can add, multiply, subtract, divide the corresponding elements in both vector

> y[3]       // Onle Third element of vector                                             
> y[-3]      // All element except third
> y[c(1,5)]  // only first and fifth element
> y[-c(1,5)]   // All except first and fifth element
> y[y<6]       // All elements less than 6
> 
> matrix(c(1,2,3,4,5,6,7,8,9), nrow=3, byrow=True)      //matrix having 3 rows and nunber is arranged row wise
> matrix(c(1,2,3,4,5,6,7,8,9), nrow=3, byrow=False)     //matrix having 3 rows and nunber is arranged column wise
> mat <- matrix(c(1,2,3,4,5,6,7,8,9), nrow=3, byrow=False)  // mat is a matrix now
> mat[1,2]                                                  // element at first row and second column
> mat[c(1,3), 2]                                            // elements at second column at first and third row both
> mat[,1]                                                   // elements at first column and at all rows
> mat*10                                                    // multiply all elements by 10

```
