# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program
```
import numpy as np
x = np.array([5, 8, 3, 7, 6])
y = np.array([2, 8, 4, 5, 6])

greater = x > y
equal = x == y

indices = np.where(x >= y)

print("x:", x)
print("y:", y)
print("\nx > y:", greater)
print("x == y:", equal)
print("\nIndices where x >= y:", indices[0])

```

## Output

![image](https://github.com/user-attachments/assets/75bc86bc-30b2-4426-bd77-1db62a960d86)

## Result
Thus the python program is successfully verified.
