# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE: 18.09.2024                                                                           
### REGISTER NUMBER : 212222060263
### AIM: 
To write a logic program to design a circuit like half adder and half subtractor.
###  Algorithm:
1. Start the Program
2. Design a AND gate logic if both inputs are 1 then output is 1.
3. Design a OR gate logic if any one of input is 1 then output is 1.
4. Design a XOR gate logic if both inputs are different then output is 1.
5. Design a NOT gate logic if input is 0 then output is 1.
6. Design a half adder and half subtractor using the rules.
7. Test the logic.
8. Stop the program.

### Program:
half_adder(A, B, Sum, Carry) :-

    Sum is (A + B) mod 2,
    
    Carry is (A + B) // 2.
    

half_subtractor(A, B, Difference, Borrow) :-

    Difference is (A - B) mod 2,
    
    Borrow is (A - B) // 2.
    

full_adder(A, B, CarryIn, Sum, CarryOut) :-

    TempSum is (A + B + CarryIn) mod 2,
    
    CarryOut is (A + B + CarryIn) // 2,
    
    Sum is TempSum.
    

full_subtractor(A, B, BorrowIn, Difference, BorrowOut) :-

    TempDiff is (A - B - BorrowIn) mod 2,
    
    BorrowOut is (A - B - BorrowIn) // 2,
    
    Difference is TempDiff.












### Output:
![image](https://github.com/user-attachments/assets/63f7f4af-8b20-401d-a7c5-efce6252934c)
![image](https://github.com/user-attachments/assets/49ae8449-6e17-4d91-921c-52d36827ad96)
![image](https://github.com/user-attachments/assets/68dc0839-a2c0-4438-b4e0-8604bade4b01)
![image](https://github.com/user-attachments/assets/c1977850-2a4a-402c-acc5-8a6a9e01a37b)






### Result:
Thus the truth table of circuit verified sucessfully.
