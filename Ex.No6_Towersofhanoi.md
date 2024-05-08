# Ex.No: 6   Logic Programming – Factorial of number   
### DATE: 09.03.2024                                                                         
### REGISTER NUMBER : 212221060027
### AIM: 
To  write  a logic program  to solve Towers of Hanoi problem  using SWI-PROLOG. 
### Algorithm:
1. Start the program
2.  Write a rules for finding solution of Towers of Hanoi in SWI-PROLOG.
3.  a )	If only one disk  => Move disk from X to Y.
4.  b)	If Number of disk greater than 0 then
5.        i)	Move  N-1 disks from X to Z.
6.        ii)	Move  Nth disk from X to Y
7.        iii)	Move  N-1 disks from Y to X.
8. Run the program  to find answer of  query.
### Program:
```
move(1,X,Y,_) :-  
    write('Move top disk from '), 
    write(X), 
    write(' to '), 
    write(Y), 
    nl. 
move(N,X,Y,Z) :- 
    N>1, 
    M is N-1, 
    move(M,X,Z,Y), 
    move(1,X,Y,_), 
    move(M,Z,Y,X).
```
### Output:
![WhatsApp Image 2024-03-24 at 9 42 44 PM](https://github.com/shanmuga2004/AI_Lab_2023-24/assets/114944625/ecc5f145-8211-4d37-bde8-acb58ecba5e4)

### Result:
Thus the solution of Towers of Hanoi problem was found by logic programming.
