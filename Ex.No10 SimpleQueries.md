# Ex.No: 10  LOGIC PROGRAMMING –  SIMPLE QUERIES FROM FACTS AND RULES

### DATE:                                                                            

### REGISTER NUMBER : 212221040011

### AIM: 

    To write a prolog program to find the answer of query. 
    
###  ALGORITHM:

    Step 1: Start the program.
    
    Step 2: Convert the sentence into First order Logic.
    
    Step 3: Convert the sentence into Horn clause form. 
    
    Step 4: Add rules and predicates in a program.
    
    Step 5: Pass the query to program.
    
    Step 6: Prolog interpreter shows the output and return answer.
    
    Step 8: Stop the program.
    
### PROGRAM:
  ### TASK - 1:
    Construct the FOL representation for the following sentences.
  
     1. John likes all kinds of food.
  
     2. Apples are food.
  
     3. Chicken is a food. 
  
     4. Sue eats everything Bill eats.
      
     5. Bill eats peanuts.
     
    Convert into clause form and Prove that John like Apple by using Prolog.
     
### PROGRAM:

    likes(john,X):- 
    food(X). 
    eats(bill,X):- 
    eats(sue,X). 
    eats(Y,X):- 
    food(X). 
    eats(bill,peanuts). 
    food(apple). 
    food(chicken). 
    food(peanuts). 

### OUTPUT:

![Experiment - 10-1](https://github.com/AKASHBKUMAR/AI_Lab_2023-24/assets/113763258/5f338f67-a7b7-4647-9355-86171d925b1a)


### TASK - 2:
    Consider the following facts and represent them in predicate form: 
    
    1. Steve likes easy courses.
    
    2. Science courses are hard.
    
    3. All the courses in Have fun department are easy.
    
    4. BK301 is Have fun department course.
    
    Convert the facts in predicate form to clauses and then prove by resolution: “Steve likes BK301 course”<br> 

### Program:

    likes(steve,X):- 
    easycourse(X). 
    hard(sciencecourse). 
    easycourse(X):- 
    course(X,dept(havefun)). 
    course(bk301,dept(havefun)).

### OUTPUT:

![Experiment - 10-2](https://github.com/AKASHBKUMAR/AI_Lab_2023-24/assets/113763258/f98fd0cb-72ea-4744-acce-d2edec17943b)

### TASK - 3:
    Consider the statement,
    
    “This is a crime for an American to sell weapons to hostile nations. The Nano , enemy of America has some missiles and its missiles were sold it by Colonal West who is an American”.
    
    Convert to Clause form and prove west is criminal by using Prolog.
### PROGRAM:

    criminal(X):- 
    american(X), 
    weapon(Y), 
    hostile(Z), 
    sells(X,Y,Z). 
    weapon(Y):- 
    missile(Y). 
    hostile(Z):- 
    enemy(Z,X). 
    sells(west,Y,nano):- 
    missile(Y), 
    owns(nano,Y). 
    missile(m). 
    owns(nano,m). 
    enemy(nano,america). 
    american(west).

### OUTPUT:

![Experiment - 10-3](https://github.com/AKASHBKUMAR/AI_Lab_2023-24/assets/113763258/04a7998f-1c35-45cc-a854-cc938de9d5c7)


### RESULT:
    Thus, the prolog programs were executed successfully and the answer of query was found.
