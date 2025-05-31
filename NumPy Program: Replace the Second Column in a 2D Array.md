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

rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))

print("Enter the elements row-wise:")
elements = []

for i in range(rows):
    row = list(map(int, input(f"Enter elements for row {i+1}, separated by space: ").split()))
    if len(row) != cols:
        raise ValueError("Incorrect number of elements.")
    elements.append(row)

original_array = np.array(elements)

print("\nEnter the new column to insert (length should be same as number of rows):")
new_column = []

for i in range(rows):
    val = int(input(f"Enter value {i+1}: "))
    new_column.append(val)

new_column_array = np.array(new_column)

array_without_second_col = np.delete(original_array, 1, axis=1)

updated_array = np.insert(array_without_second_col, 1, new_column_array, axis=1)

print("\nOriginal Array:")
print(original_array)

print("\nUpdated Array with new column at index 1:")
print(updated_array)

```

## Output

![image](https://github.com/user-attachments/assets/612e992e-69a6-4587-9bb6-d346a0a26406)

## Result
Thus the python program is successfully verified.
