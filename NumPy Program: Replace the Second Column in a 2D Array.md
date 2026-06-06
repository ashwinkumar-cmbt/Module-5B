# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program

```
import numpy as np

# Input 2D array
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter elements of array:")
arr = []
for i in range(rows):
    arr.append(list(map(int, input().split())))

a = np.array(arr)

# Input new column
print("Enter new column elements:")
new_col = list(map(int, input().split()))
new_col = np.array(new_col).reshape(rows, 1)

# Delete second column (index 1)
deleted = np.delete(a, 1, axis=1)

# Insert new column at position 1
result = np.insert(deleted, 1, new_col, axis=1)

print("Original Array:")
print(a)

print("Updated Array:")
print(result)
```

## Output

<img width="372" height="315" alt="image" src="https://github.com/user-attachments/assets/62e0b3ba-9040-4eaf-8edb-c96b25cf5d93" />


## Result

The program is excuted successfully and the output is verified.

