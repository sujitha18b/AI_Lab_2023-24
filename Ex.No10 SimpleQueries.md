# Ex.No: 10  Logic Programming –  Simple queries from facts and rules
### DATE: 9.10.2024                                                                     
### REGISTER NUMBER : 212222060263
### AIM: 
To write a prolog program to find the answer of query. 
###  Algorithm:
 Step 1: Start the program <br> 
 Step 2: Convert the sentence into First order Logic  <br> 
 Step 3:  Convert the sentence into Horn clause form  <br> 
 Step 4: Add rules and predicates in a program   <br> 
 Step 5:  Pass the query to program. <br> 
 Step 6: Prolog interpreter shows the output and return answer. <br> 
 Step 8:  Stop the program.
### Program:
### Task 1:
Construct the FOL representation for the following sentences <br> 
1.	John likes all kinds of food.  <br> 
2.	Apples are food.  <br> 
3.	Chicken is a food.  <br> 
4.	Sue eats everything Bill eats. <br> 
5.	 Bill eats peanuts  <br> 
   Convert into clause form and Prove that John like Apple by using Prolog. <br> 
### Program:
likes(john, X) :- food(X).

food(apple).

food(chicken).

eats(sue, X) :- eats(bill, X).

eats(bill, peanuts).


### Output:
![image](https://github.com/user-attachments/assets/9652793a-e7b9-4df7-a214-a31a95c204d4)

### Task 2:
Consider the following facts and represent them in predicate form: <br>              
1.	Steve likes easy courses. <br> 
2.	Science courses are hard. <br> 
3. All the courses in Have fun department are easy <br> 
4. BK301 is Have fun department course.<br> 
Convert the facts in predicate form to clauses and then prove by resolution: “Steve likes BK301 course”<br> 

### Program:
have_fun_course(bk301).

likes(steve, X) :- easy(X).

easy(X) :- have_fun_course(X).

### Output:
![image](https://github.com/user-attachments/assets/354ed280-693c-4ff9-b95b-544cbc9cd178)


### Task 3:
Consider the statement <br> 
“This is a crime for an American to sell weapons to hostile nations. The Nano , enemy of America has some missiles and its missiles were sold it by Colonal West who is an American” <br> 
Convert to Clause form and prove west is criminal by using Prolog.<br> 
### Program:
hostile(nano).

american(west).

missile(missile1).

sells(west, missile1, nano).

criminal(X) :- american(X), sells(X, Y, Z), missile(Y), hostile(Z).


### Output:
![image](https://github.com/user-attachments/assets/ae6fd94f-96ad-4938-9c22-b6145f200bd3)

### Result:
Thus the prolog programs were executed successfully and the answer of query was found.
