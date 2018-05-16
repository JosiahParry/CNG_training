Introduction to R
========================================================
author: Josiah Parry
date: 
autosize: true

What is R
========================================================

* R is a statistical programming language.
* It does statistics and a few other things.
* But it does statistics very well.
* It's not like any other programming language you've used. 


Installing R & RStudio
=====================================================

Go to the **Comprehensive R Archive Network (CRAN)** and download R
- https://cran.r-project.org/

Download RStudio **_desktop_** 
- https://www.rstudio.com/products/rstudio/download2/


RStudio Environment
========================================================


![RStudio Environment](cng/images/environment.png)

R as a Calculator
========================================================
R Follows the order of operations




```r
1 + 1 # addition

2 - 1 # subtraction

10 * 10 # multiplication

32 / 4 # division

10^2 # powers
```


```r
(100^10)^(1/10)
```

```
[1] 100
```

R as a Calculator Continued
=======================================

Just like we do in algebra, we can assign values to variables and do math with variables. 

```r
x <- 10
y <- 35

x * y
```

```
[1] 350
```

```r
x / y
```

```
[1] 0.2857143
```



Data Types
=======================================
* Numeric
  - Integer: `int` for short, is any whole number, specified with an `L`
      - `x <- 10L`
  - Double: `dbl` for short, is any number with a decimal
      - `y <- 2.7182818284590452353602874713527`
* Character / String
  - `chr` for short is anything surrounded by quotations. These are generally words or expressions.
      - `string <- "this is a character string"`
* Logical
  - `TRUE`  or  `FALSE`  or  `NA`  or  `NULL`


Logical Comparisons
=========================================

## _Life is not black and white_
## _Life is not binary_

We can think of these as logical statements.

When we think of binary we think of ones and zeros. Where 1 is true, and 0 is false. 





Data Structures
========================================================

* **vectors**
  - This is a collection of observations of the same data type
  - Think of this as a column in an excel or SQL table
* **data frames**
  - A collection of vectors of the same length
  - Think of this as an excel / SQL table
  
Vectors
========================================================

* Use the `c()` (combine) function. 
* Each value is separated by a comma: `c("value 1", "value 2")`
    

```r
numeric_vector <- c(1, 2, 3, 4, 5)
character_vector <- c("Camp", "NextGen", "is awesome!")

numeric_vector
```

```
[1] 1 2 3 4 5
```

```r
character_vector
```

```
[1] "Camp"        "NextGen"     "is awesome!"
```

Vectors Example
========================================================

You can preform operation on each element of a vector, so long as its _"legal"_

```r
numeric_vector - 3 
```

```
[1] -2 -1  0  1  2
```


```r
character_vector - 3
```

```
Error in character_vector - 3 : non-numeric argument to binary operator
```
Vectors Example 2 
========================================================
Can you mix types?


```r
mixed_vector <- c(TRUE, 1, "mIxeDD VecT0rr")
mixed_vector
```

```
[1] "TRUE"           "1"              "mIxeDD VecT0rr"
```

Notice how every value is automatically converted to a character string. Be careful with your data types! 

Data Frames
============================

This is a built in dataset stored as a `tibble` (a fancy data frame).
Above each column is a description of column types. Notice the difference between `int` and `dbl`
  

```
# A tibble: 6 x 5
  name           height  mass homeworld species
  <chr>           <int> <dbl> <chr>     <chr>  
1 Luke Skywalker    172   77. Tatooine  Human  
2 C-3PO             167   75. Tatooine  Droid  
3 R2-D2              96   32. Naboo     Droid  
4 Darth Vader       202  136. Tatooine  Human  
5 Leia Organa       150   49. Alderaan  Human  
6 Owen Lars         178  120. Tatooine  Human  
```


Packages & the Tidyverse
========================================================

Reading Flat Files 
========================================================


The Pipe Operator
========================================================


Using R like it's SQL
========================================================

* Select
* Filter
* Mutate (columnwise computation)

Reading data from Google Sheets
========================================================

Aggregating Data
========================================================
* `group_by()`
* `count()`
* `summarise()`

Exercises
========================================================

Calculate % to goal for 3 metrics


Chart Making with ggplot2
========================================================

