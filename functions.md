
### sample()
randomization. like shuffle. after it you can take first or last n elements.


###  rbind()
adding two `dataframe` in row wise. so columns must be same in two dataframe

###  match()
 return the index of occurance of element of first vector in the second vector.
    
    print(match(5, c(1,2,9,5,3,6,7,4,5)))
    [1] 4
    
    > v1 <- c("a1","b2","c1","d2")
    > v2 <- c("g1","x2","d2","e2","f1","a1","c2","b2","a2")
    > x <- match(v1,v2)
    > x
    [1] 6 8 NA 3
    
match() can be equivalent of %in%. difference is that %in% return True/False, and match() returns the number.

    > v1 <- c("a1","b2","c1","d2")
    > v2 <- c("g1","x2","d2","e2","f1","a1","c2","b2","a2")
    > v1 %in% v2
    [1] TRUE TRUE FALSE TRUE
`nomatch = 0` parameter defines the integer to be sent if there is no match for a element in vec1 in the vec2.




   > v1 <- c("a1","b2","c1","d2")
   > v2 <- c("g1","x2","d2","e2","f1","a1","c2","b2","a2")
   > x <- match(v1,v2, nomatch = 0)
   > x
   [1] 6 8 0 3
   
### table() function
[link](https://www.r-bloggers.com/r-function-of-the-day-table/)
   
   
### formula()
it contains various operator to setup the equation for regression. [very detailed one](https://www.datacamp.com/community/tutorials/r-formula-tutorial)
   
   
   
## ggplot2
### qplot()
basic ggplot, but with more flexibility. a working example in [here](http://www.sthda.com/english/wiki/qplot-quick-plot-with-ggplot2-r-software-and-data-visualization)
## installing packages
    if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

    BiocManager::install("apeglm")
### from others
    
    install.packages('dowloader')

## get the absoulte path of the currently executing path

    paste0(gsub("\\", "/", fileSnapshot()$path, fixed=TRUE),"/")
