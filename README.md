# Suduko-Solver
#USING BACKTRACKING 

Like all other Backtracking problems, Sudoku can be solved by assigning numbers one by one to empty cells. Before assigning a number, check whether it is safe to assign. 

Check that the same number is not present in the current row, current column and current 3X3 subgrid. After checking for safety, assign the number, and recursively 
       check whether this assignment leads to a solution or not. If the assignment doesn’t lead to a solution, then try the next number for the current empty cell.
       And if none of the number (1 to 9) leads to a solution, return false and print no solution exists.


Follow the steps below to solve the problem:

> Create a function that checks after assigning the current index the grid becomes unsafe or not. Keep Hashmap for a row, column and boxes. If any number has a frequency greater than 1 in the hashMap return false else return true; hashMap can be avoided by using loops.
> Create a recursive function that takes a grid.
> Check for any unassigned location. 
> If present then assigns a number from 1 to 9.
> Check if assigning the number to current index makes the grid unsafe or not. 
> If safe then recursively call the function for all safe cases from 0 to 9.
> If any recursive call returns true, end the loop and return true. If no recursive call returns true then return false.
> If there is no unassigned location then return true.

SCREENSHOT:-

![alt text](https://user-images.githubusercontent.com/88509277/202609247-69ee7268-60d0-4760-b43b-4baaf9d2c366.png)
![Suduko Solver Filled](https://user-images.githubusercontent.com/88509277/202609529-aad55671-da0b-4369-9e0d-43f9a6d9385e.png)



