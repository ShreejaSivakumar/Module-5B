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
print(f"Enter {rows * cols} elements row-wise (separated by space):") 
elements = list(map(int, input().split()))
original_array = np.array(elements).reshape(rows, cols)
print("\nOriginal Array:") 
print(original_array)
print(f"\nEnter {rows} elements for the new column:") 
new_column = list(map(int, input().split()))
array_without_second_col = np.delete(original_array, 1, axis=1)
updated_array = np.insert(array_without_second_col, 1, new_column, axis=1)
print("\nUpdated Array (with second column replaced):") 
print(updated_array)
```

<img width="881" height="322" alt="Screenshot 2026-06-05 210430" src="https://github.com/user-attachments/assets/987f847f-60a6-4e68-ac4e-55ca57a8c627" />


## Output
<img width="580" height="407" alt="Screenshot 2026-06-05 210437" src="https://github.com/user-attachments/assets/52923a9f-f6db-449d-8daf-c129d512ef08" />

## Result
Thus To write a NumPy program that deletes the second column from a given 2D array and inserts a new column at the same position. Hence the code has been executed successfully.
