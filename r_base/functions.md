`unique()`    
`duplicated()`   
`anyDuplicated()`
these functions are used for checking duplicates in the vector. inputs are `vectors`
  
        x <- 1:10
        names(x) <- letters[1:10]
        anyDuplicated(names(x))
        > [1] 0 # means no duplication
