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
Add code here
```
import numpy as np
rows = int(input("Enter number of rows: ")) 
cols = int(input("Enter number of columns: "))

print(f"Enter {rows * cols} elements row-wise (separated by space):") 
elements = list(map(int, input().split()))

original_array = np.array(elements).reshape(rows, cols)

sorted_array = np.sort(original_array, axis=0)

print("\nOriginal Array:\n", original_array) 
print("\nColumn-wise Sorted Array:\n", sorted_array)

```
<img width="777" height="311" alt="Screenshot 2026-06-05 210052" src="https://github.com/user-attachments/assets/228d970d-5db2-429f-b100-3777eaa801ac" />

## Output
<img width="575" height="337" alt="Screenshot 2026-06-05 210058" src="https://github.com/user-attachments/assets/88bd127e-c71d-4933-94f6-0f46f319f92d" />

## Result
Thus To write a NumPy program that sorts the elements in each column of a given 2D array in ascending order. Hence the code has been executed successfully.
