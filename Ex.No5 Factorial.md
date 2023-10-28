# Ex.No: 5   LOGIC PROGRAMMING – FACTORIAL OF A NUMBER  
### DATE:                                                                            
### REGISTER NUMBER : 212221040011
### AIM: 
    To  write  a logic program for finding the factorial of given number using SWI-PROLOG.
    
### ALGORITHM:

    1. STEP 1: Start the program.
    
    2. STEP 2:  Write a rules for finding factorial of given program in SWI-PROLOG.
    
    3.   a)	factorial of 0 is 1 => written as factorial(0,1).
    
    4.   b)	factorial of number greater than 0 obtained by recursively calling the factorial function.
    
    5. STEP 3: Run the program  to find answer of  query.
    
    6. STEP 4: Stop the program.

### PROGRAM:

    factorial(0,1). 
    factorial(A,B) :-   
    A > 0,  
    C is A-1, 
    factorial(C,D), 
    B is A*D. 


### OUTPUT:

![Experiment - 05](https://github.com/AKASHBKUMAR/AI_Lab_2023-24/assets/113763258/cf4cc2f4-3af5-4464-9229-f89faa7a0b74)


### RESULT:

    Thus, the factorial of given number was found by logic programming. 
