
[Bioconductor by Hens](https://leanpub.com/bioconductor)

# objects in R:
1.  numeric
2.  integer
3.  character
4.  factor
5.  logical

# Integers
default representation of number in R is **numeric**, **not** integer.


    x <- 1
    class(x)
    > "numeric"
    
    x <- 1:3
    class(x)
    > "integer"
    
to make sure to get integer in R, we can append `L` to the number

x <- 1L
class(x)
> [1] "integer"

**numeric can hold larger value than integer**


# Matrix
`matrix` contains same type of values

`dim(matrix a)` is like `np.shape`

If you grab a single row or a single column from a you get a vector matrix  
Sometimes, it is really nice to get a **matrix**; you do that by using `drop=FALSE` in the subsetting:

      x[1,] # get the first row but in the vector form
      > [1] 1 4 7
      x[1,, drop = FALSE] # retrun matrix form of row 1
      > 
  
I am a heavy user of the package **matrixStats**² for
the full suite of `rowXX` and `colXX` with `XX` being any standard statistical function such as `sd()`, `var()`,
`quantiles()` etc.

Internally, a matrix is just a `vector with a dimension attribute`. In R we have `column-first
orientation`, so the **columns are filled up first:**


      > matrix(1:9, 3, 3)
          [,1] [,2] [,3]
          [1,] 1 4 7
          [2,] 2 5 8
          [3,] 3 6 9
      > matrix(1:9, 3, 3, byrow = TRUE)
          [,1] [,2] [,3]
          [1,] 1 2 3
          [2,] 4 5 6
          [3,] 7 8 9
          
          
 # List
 
 lists are like vectors, but can hold together objects of arbitrary kind.
   
   
    > x <- list(1:3, letters[1:3], is.numeric)
    > x
        [[1]]
          [1] 1 2 3
        [[2]]
          [1] "a" "b" "c"
        [[3]]
          function (x) .Primitive("is.numeric")
          
    > names(x) <- c("numbers", "letters", "function")
    > x[1:2]
        $numbers
          [1] 1 2 3
        $letters
          [1] "a" "b" "c"
    > x[1]
        $numbers
          [1] 1 2 3
        > x[[1]]
          [1] 1 2 3
          
          
          
          
 indexing in the list
 
 `x[[1]]`  integer based indexing. give the content of the elements in that index
 
          > x[[1]]
            [1] 1 2 3
          
`x[1]` or `x["numbers"] give the name of that index along with content. x[1]$   give the names of that index.

        > x[1]
          $numbers
          [1] 1 2 3
          
        > x[1]$number
 `x[[1]]` or `x[["numbers"]]` give the content only
    
    
          > x[[1]]
            [1] 1 2 3
            
            
 if the list is named,then x$numbers is equivalent to x[['numbers']]
 
 
          > x$letters
            [1] "a" "b" "c"
            
          > x["letters"]
 
          > x$letters
          [1] "a" "b" "c"
          
          > x["letters"]
          $letters
          [1] "a" "b" "c"
          
          > x$let
          [1] "a" "b" "c"
          > x["let"]
          $<NA>
          NULL
 
        
        
# DataFrame
 They look like matrices, but each column can be a
separate type, so you can mix and match different data types. They are required to have unique
column and row names. If no rowname is given, itâ€™ll use 1:nrow.
  


       x[
       x[1:2] # integer based slicing
       
       x[
