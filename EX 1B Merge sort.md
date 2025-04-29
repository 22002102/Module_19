# EX1_B : B.Merge Sort 
## DATE: 25/02/2025
## AIM:
To write a python program to sort the first half of the list using merge sort.

## Algorithm
1.Input a list of n numbers and store them in a list li.

2.Divide the list into two halves: left_sort and right_sort, until each sublist has one or zero elements.

3.Recursively sort both halves by calling the mergesort() function on each.

4.Merge the two sorted halves into the original list li by comparing elements from both halves and inserting the smaller one.

5.Output the final sorted list after all merge steps are completed.

## Program:
```
/*
Developed by: SANJAY S
RegisterNumber:212222230132
*/

def mergesort(li):
    if len(li) <= 1:
        return li
        
    mid = len(li)//2
    left_sort = li[:mid]
    right_sort = li[mid:]
        
    mergesort(left_sort)
    mergesort(right_sort)
        
    i = j = k = 0
        
    while i < len(left_sort) and j < len(right_sort):
        if left_sort[i] < right_sort[j]:
            li[k] = left_sort[i]
            i+=1
        else:
            li[k] = right_sort[j]
            j+=1
        k+=1
        
    while i < len(left_sort):
        li[k] = left_sort[i]
        i+=1
        k+=1
            
    while j < len(right_sort):
        li[k] = right_sort[j]
        j+=1
        k+=1

li = []    
num = int(input())
for _ in range(num):
    li.append(int(input()))
mergesort(li)
print(li)
```

## Output:

![image](https://github.com/user-attachments/assets/7ab4a0aa-14b0-408a-a6eb-74ae15a05c8c)




## Result:
Thus, the Python program to implement Merge Sort for sorting a list of numbers is implemented successfully.
