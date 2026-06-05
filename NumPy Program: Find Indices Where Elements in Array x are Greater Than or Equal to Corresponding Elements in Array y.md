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

Add code here
```
import numpy as np

x = np.array([10, 20, 30, 40, 50]) 
y = np.array([15, 20, 25, 35, 60])
greater_than = x > y 

equal_to = x == y
condition = x >= y 
indices = np.where(condition)
print("x:", x) 
print("y:", y) 
print("x >= y condition:", condition) 
print("Indices where x >= y:", indices[0])
```
<img width="533" height="281" alt="Screenshot 2026-06-05 210208" src="https://github.com/user-attachments/assets/ef17de85-2a5d-4f74-b437-adf5bbda29fd" />
## Output
<img width="505" height="138" alt="Screenshot 2026-06-05 210213" src="https://github.com/user-attachments/assets/ad39c549-9b7e-45ff-8c03-6dfe819c7b98" />

## Result
Thus To write a Python program using NumPy that finds the indices where elements in array x are greater than or equal to their corresponding elements in array y. Hence the code has been executed successfully.
