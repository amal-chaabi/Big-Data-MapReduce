# Big-Data-MapReduce
#Amal Chaabi



Execute : 
hadoop fs -put numbers.txt numbersFile
hadoop jar NumbersDemo.jar NumbersPackagDemo.NumberCount numbersFile MRDir1 MRDir2
hadoop fs -ls MRDir1
hadoop fs -ls MRDir2
hadoop fs -cat MRDir1/part-r-00000
hadoop fs -cat MRDir2/part-r-00000

numberFile: input file 
MRDir1 : output of the first job to count odd and even numbers  , the result will be like 0 4     // there are 4 even numbers and 4 odd numbers
                                                                                          1 4
MRDir89 : output of the second job  to sum the odd numbers and even numbers , the result will be like 0 20      // sum of even numbers=20 and sum of odd numbers=32
                                                                                                      1 32 
                                                                                                      
                               0 means even numbers 
                               1 means odd numbers 
