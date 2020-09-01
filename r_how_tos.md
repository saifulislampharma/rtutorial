## how to install a package

    install.packages("package_name)
    
there are a lot of options to this method. like c++


## how to load a library
    library(package Name)

## how to see all the loaded library

    library()
  
## only base packages
  
    library(lib.loc = .Library)
  
## how to get the name of methods in a given package

    library(help = splines)
## how to get structure of an object

    str(obj_name)
    # can also use 
    summary(obj_a)
    
## how to see the files in current directory

    dir()
    
## how to find a specific pattern in current directory
    ls(pat = "specific_pattern)

## how many data types are there
![r](r_data_types.jpg)


## setting name attributes 
    
    names(obj) <- value
    
    # or if u want to see the names
    
    names(obj)
    
## Data Structures
![data structure](r_data_structures.jpg)


## what is order of corercion
The ordering is roughly logical < integer < numeric < complex < character
so logical will be integer

## to check class of any object

    class(obj_name)
    
## if have time, investigate the typeof() function


## how to initialize vectors
![vector initialization](r_vectors_init.jpg)

## how to index vectors
the upper limit of the range is also included in the result
![vector index](r_vectors_index.jpg)

![vector index](r_vectors_index2.jpg)

## how to reverse elements of a vector
    
    rev(x)
## how to replicate 

    rep(1,9)
    >[1] 1 1 1 1 1 1 1 1 1
## Matrix initialization
![matrix initialization](r_matrix_init.jpg)

![matrix initialization2](r_matrix_init2.jpg)
![matrix iop](r_matrix_op2.jpg)


## list initialization
![list_initit](images/r_list_ini.jpg)

## list operation
`ls[[1]]` and `ls$a` return the same type of data. but `ls[1]` return a list
![list_operaton](images/r_list_op.jpg)

![list_operaton2](images/r_list_op1.jpg)
