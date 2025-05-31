# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
```
import pandas as pd
import numpy as np

exam_data = {
    'name': ['Anu', 'Bala', 'Catherine', 'David', 'Eva', 'Frank', 'Grace', 'Hannah'],
    'score': [85, 76, 90, 60, 45, np.nan, 77, 88],
    'attempts': [1, 3, 2, 3, 2, 1, 2, 1],
    'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'yes']
}

labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h']

df = pd.DataFrame(exam_data, index=labels)

print("Exam Data DataFrame:\n")
print(df)

```
## Output

![image](https://github.com/user-attachments/assets/471a60bf-6d12-44e4-b62d-69f983e7cb7e)

## Result
Thus the python program is successfully verified.
