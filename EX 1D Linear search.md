# EX1_D : Linear Search 
## DATE: 25/02/2025
## AIM:
To write a python program for a search function with parameter list name and the value to be searched using string values.

## Algorithm
1. Input a list of n elements and store them in List.

2. Input the element x to be searched.

3. Check if x is present in List using the in operator.

4. If found, return 'Found'.

5. Else, return 'Not Found'.

## Program:
```
Write a python program for a search function with parameter list name and the value to be searched on the given list of int values.
/*
Developed by: SANJAY S
RegisterNumber:212222230132
*/

def search(List,x):
    if x in List:
        return 'Found'
    else:
        return 'Not Found'
        
List = []
n = int(input())
for i in range(n):
    List.append(int(input()))
x = int(input())
print(search(List, x))
```

## Output:

![image](https://github.com/user-attachments/assets/1d172bd7-4f06-4033-b25a-08916084ecbb)


## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list, printing "Found" if the element exists or "Not Found" if it does not.
