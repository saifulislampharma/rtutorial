
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
