# EX1_C : Quick Sort 
## DATE: 25/02/2025
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of float values.

## Algorithm
1. Input a list of n elements and store them in arr.

2. Choose a pivot element (here, the middle element of the list).

3. Partition the list into three sublists:

    - left: elements less than the pivot

    - middle: elements equal to the pivot

    - right: elements greater than the pivot

4. Recursively apply the quick sort function to left and right sublists.

5. Return the concatenated result of sorted left, middle, and sorted right.

## Program:
```
Write a python program to implement quick sort using random pivot value.
/*
Developed by: SANJAY S
RegisterNumber:212222230132
*/

def quick_sort(arr):
    if len(arr) <= 1:
        return arr
    else:
        pivot_index = len(arr) // 2
        pivot = arr[pivot_index]
        left = [x for x in arr if x < pivot]
        middle = [x for x in arr if x == pivot]
        right = [x for x in arr if x > pivot]
        return quick_sort(left) + middle + quick_sort(right)
        
arr = []
size = int(input())
for _ in range(size):
    arr.append(int(input()))
sorted_arr = quick_sort(arr)
print(sorted_arr)
```

## Output:

![image](https://github.com/user-attachments/assets/728d1f9d-d095-4425-b775-bdd543310ed1)



## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
