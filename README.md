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
 mpg cyl  disp  hp drat    wt  qsec vs am gear carb  
Mazda RX4           21.0   6 160.0 110 3.90 2.620 16.46  0  1    4    4  
Mazda RX4 Wag       21.0   6 160.0 110 3.90 2.875 17.02  0  1    4    4  
Datsun 710          22.8   4 108.0  93 3.85 2.320 18.61  1  1    4    1  
Hornet 4 Drive      21.4   6 258.0 110 3.08 3.215 19.44  1  0    3    1  
Hornet Sportabout   18.7   8 360.0 175 3.15 3.440 17.02  0  0    3    2  
Valiant             18.1   6 225.0 105 2.76 3.460 20.22  1  0    3    1
Duster 360          14.3   8 360.0 245 3.21 3.570 15.84  0  0    3    4
Merc 240D           24.4   4 146.7  62 3.69 3.190 20.00  1  0    4    2
Merc 230            22.8   4 140.8  95 3.92 3.150 22.90  1  0    4    2
Merc 280            19.2   6 167.6 123 3.92 3.440 18.30  1  0    4    4
Merc 280C           17.8   6 167.6 123 3.92 3.440 18.90  1  0    4    4
Merc 450SE          16.4   8 275.8 180 3.07 4.070 17.40  0  0    3    3
Merc 450SL          17.3   8 275.8 180 3.07 3.730 17.60  0  0    3    3
Merc 450SLC         15.2   8 275.8 180 3.07 3.780 18.00  0  0    3    3
Cadillac Fleetwood  10.4   8 472.0 205 2.93 5.250 17.98  0  0    3    4
Lincoln Continental 10.4   8 460.0 215 3.00 5.424 17.82  0  0    3    4
Chrysler Imperial   14.7   8 440.0 230 3.23 5.345 17.42  0  0    3    4
Fiat 128            32.4   4  78.7  66 4.08 2.200 19.47  1  1    4    1
Honda Civic         30.4   4  75.7  52 4.93 1.615 18.52  1  1    4    2
Toyota Corolla      33.9   4  71.1  65 4.22 1.835 19.90  1  1    4    1
Toyota Corona       21.5   4 120.1  97 3.70 2.465 20.01  1  0    3    1
Dodge Challenger    15.5   8 318.0 150 2.76 3.520 16.87  0  0    3    2
AMC Javelin         15.2   8 304.0 150 3.15 3.435 17.30  0  0    3    2
Camaro Z28          13.3   8 350.0 245 3.73 3.840 15.41  0  0    3    4
Pontiac Firebird    19.2   8 400.0 175 3.08 3.845 17.05  0  0    3    2
Fiat X1-9           27.3   4  79.0  66 4.08 1.935 18.90  1  1    4    1
Porsche 914-2       26.0   4 120.3  91 4.43 2.140 16.70  0  1    5    2
Lotus Europa        30.4   4  95.1 113 3.77 1.513 16.90  1  1    5    2
Ford Pantera L      15.8   8 351.0 264 4.22 3.170 14.50  0  1    5    4
Ferrari Dino        19.7   6 145.0 175 3.62 2.770 15.50  0  1    5    6
Maserati Bora       15.0   8 301.0 335 3.54 3.570 14.60  0  1    5    8
Volvo 142E          21.4   4 121.0 109 4.11 2.780 18.60  1  1    4    2
