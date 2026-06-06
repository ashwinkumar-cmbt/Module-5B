# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program

```
import numpy as np

# Accept 2D array input
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter elements:")
arr = []

for i in range(rows):
    row = list(map(int, input().split()))
    arr.append(row)

a = np.array(arr)

# Column-wise sorting
sorted_arr = np.sort(a, axis=0)

print("Original Array:")
print(a)

print("Column-wise Sorted Array:")
print(sorted_arr)

```

## Output

<img width="478" height="326" alt="image" src="https://github.com/user-attachments/assets/e5aa3a54-4fbb-42f2-957f-fff513f2738a" />


## Result

The program is excuted successfully and the output is verified.

