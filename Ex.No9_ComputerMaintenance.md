# Ex.No: 9  LOGIC PROGRAMMING –  COMPUTER MAINTENANCE EXPERT SYSTEM
### DATE:                        

### REGISTER NUMBER : 212221040011

### AIM: 
     To write a Prolog program to build a computer maintenance expert system.
     
###  ALGORITHM:

     1. Start the program.
     
     2. Write the rules for each fault in computer.
     
     3. If system have printing problem, missing dots and no uniform printing then system fault on printer head.
     
     4. If system have not printing, missing dots and spread inks then system fault on ribbon.
     
     5. If system have not printing, paper jam and out of paper then system fault on paper stuck in printer.
     
     6. Similarly define rules for all faults.
     
     7. Define facts for system problems.
     
     8. Find the fault of computer by passing query to system.
     
### PROGRAM:

     fault(printer_head) :- 
     problem(not_printing), 
     problem(missing_dots), 
     problem(nonuniform_printing). 
     fault(ribbon) :- 
     problem(not_printing), 
     problem(missing_dots), 
     problem(spread_ink). 
     fault(paper) :- 
     problem(not_printing), 
     problem(paper_jam), 
     problem(out_of_paper). 
     fault(motherboard) :- 
     problem(long_beep), 
     problem(short_beep). 
     fault(hard_disc) :- 
     problem(two_short_beeps), 
     problem(blank_display). 
     problem(not_printing). 
     problem(missing_dots). 
     problem(spread_ink). 
     problem(two_short_beeps). 
     problem(blank_display). 

### OUTPUT:

![Experiment - 09](https://github.com/AKASHBKUMAR/AI_Lab_2023-24/assets/113763258/0f04ac56-ecd4-4a2a-b280-cdef4e5405fd)



### RESULT:
     Thus, the simple omputer maintenance expert system was built sucessfully.
