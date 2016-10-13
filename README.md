# R-projects
projects to get started with R programming.

STEPS:
  - 1. Download R from CRAN https://cran.cnr.berkeley.edu/STEP 
  - 2. Download R Studio. from https://www.rstudio.com/products/rstudio/download3/

setup working directory.
> Open R -> Misc -> Change Working Directory. {Create and set your working directory, default for these projects.}
> Inside R Console  check the directory set by typing

```sh
$ getwd()
## to set directory manually 
$ setwd('path to directory')
```

Basic usage in R
    ##Exercies is meant for the user to run
```sh
## This is a comment
x <- 5   ## Assignment
x        ## Prints x ; Exercise

y <- 1:26  ## creates a sequence from 1 through 26 Creates a VECTOR
y          ## Exercies.

```

Objects in R (character, numeric -real number, integer, complex, logical(T/F))
```sh
## create a vector (contains same type), exception list (this can contain multiple types)
vector()

## Number, Default behaviour is two precision.
x <- 5  ##( x is 5.00)

## Integer
z <- 7L ##(z is 7)

## Infinity  - (this is a special number)
Inf

## NaN - is a special number 'Not a Number'
0/0

############### VECTOR ####################
##1. c()  function to create vector
x <- c(T, F)                                            ## boolean
x <- c("sandeep","svara", "aadya", "rajni", "kandekar") ## char
x <- 7:29                                               ## integer
x <- c(1+0i 2+3i)                                       ## complex number. i is immaginary part of complex num.

##2. vector()  function to create vector
x <- vector(numeric, length = 10)
x    ##Exercise  initialized with 0s

## be careful of coersion when creating mixed object vector.

## LIST
x <- list(35, "sandeep", FALSE, 89+7i)
x  ## Exercise

############## MATRIX #####################
## Matrix is a special kind of Vector, which has dimension.
m <- matrix(1:6, nrow  = 2, ncol = 3)  ##creates column wise.
m  ## Exercise

m <- 1:10
dim(m) <- c(2,5)  ## take teh vector m, and transform it into a matrix with 2 rows and 5 columns
m  ## Exercise

c-bind
x <- 3:5
y <- 13:15

cbind(x,y)  ## creates matrix with 3,4,5 in rows
rbind(x,y)  ## creates matrix with 3,4,5 in column
 




##NaN is Na but converse is not true.
x<- c(1,2,NaN,NA,4)
is.na(x)  ##FALSE FALSE TRUE TRUE FALSE
is.nan(x) ##FALSE FALSE TRUE FALSE FALSE


##################################################################
##Data Frames - used to store tabular data.
read.table()  or read.csv()    | data.matrix() converts to matrix.

x <- data.frame(foo = 1:4, bar = c(T,T,F,F))
x  ## Exercise.





```