# Homework2

#### Please design questions suitable for an upper level undergraduate course to illustrate the concepts we covered in class. Then, provide the answer key for your own questions (i.e. answer your own questions). Below, a prompt is given for the concept you are to design a question from. When given an option, try your best to choose the one that you're least familiar with so you can hone your own understanding.

1. Ask a question that requires a student to understand naigation and manipulation of dirctories in a filesystem. Your question should require an anser using at least the following commands/ concepts: cd, ../, mkdir, rmdir 
  * **Question:** Create a directory called "emotion" on to your home directory and inside the "emotion" directory create two directories called "happy" and "sad". Again inside the "happy" directory create "my pet". Then remove "sad" directory. After doing this, check out whether this actually worked. 

  * **Answer:**
  > $ mkdir ~/emotion  
    $ cd emotion  
    $ mkdir happy  
    $ mkdir sad  
    $ cd happy  
    $ mkdir mypet  
    $ cd ../  
    $ rmdir sad  
    $ ls emotion  

"$ ls emotion" will help you to check whether this procedure worked. This shows the directory called happy only because I remove "sad" directory from "emotion" 

2. Ask a question that requires a student to understand the difference between accessing a column in a matrix with numeric indices versus accessing a column in a data frame with numeric indices. Your question should require an answer comparing the following: mymatrix[,1] vs. mydf[,1] vs. mydf[1] vs. mydf[[1]].
  * **Question:** Create 3 by 4 matrix with entries of 1 through 12 by row and give the matrix name it as mymatrix. Then create or import or use the built in data frame and name it as mydf. Compare mymatrix[,1] vs. mydf[,1] vs. mydf[1] vs. mydf[[1]].
  * **Answer:**
  > mymatrix <-matrix(c(1:12),3,4,byrow=TRUE)  
    mymatrix  
          [,1] [,2] [,3] [,4]  
   [1,]    1    2    3    4  
   [2,]    5    6    7    8  
   [3,]    9   10   11   12  
  > mydf <-mtcars 
