# EX1_A : Reverse a String 
## DATE: 25/02/2025
## AIM:
To write a program to create a recursive function to reverse a string.

## Algorithm
1. Start with an input string reverseme.

2. Check if the string is empty; if yes, return it as is.

3. Take the last character of the string.

4. Recursively call the function on the remaining substring (excluding the last character).

5. Return the last character + result of the recursive call.

## Program:
```
/*
Developed by: SANJAY S
RegisterNumber:212222230132
*/

def reverse(reverseme):
    if len(reverseme) < 1:
        return reverseme
    else:
        return reverseme[-1]+ reverse(reverseme[:-1])
reverseme = input()
print(reverse(reverseme))
```

## Output:

![image](https://github.com/user-attachments/assets/d3aa6049-071a-4c9f-bb4b-55408e2813a5)



## Result:
Thus, the Python program to implement string reversal using recursion is implemented successfully.
