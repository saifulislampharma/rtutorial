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
