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

--------------------------------------------------------------------------------------------
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

----------------------------------------------------------------------------------------

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

------------------------------------------------------------------------------------

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

exam_data = { 'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily'], 'score': [12.5, 9, 16.5, np.nan, 9], 'attempts': [1, 3, 2, 3, 2], 'qualify': ['yes', 'no', 'yes', 'no', 'no'] }

labels = ['a', 'b', 'c', 'd', 'e']

df = pd.DataFrame(exam_data, index=labels)

print(df)
```

## Output

<img width="422" height="150" alt="Screenshot 2026-06-05 210601" src="https://github.com/user-attachments/assets/1112b9b2-2e6c-49d4-9b51-25dfb1269138" />


## Result
Thus To create and display a DataFrame using the Pandas library in Python from a given dictionary, and apply specific index labels to the rows. Hence the code has been executed successfully.

----------------------------------------------------------------------------------------

# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program

Add code here
```
import pandas as pd

student_data1 = { 'student_id': ['S1', 'S2', 'S3', 'S4'], 'name': ['Alice', 'Bob', 'Charlie', 'David'], 'marks': [85, 90, 95, 80] }

student_data2 = { 'student_id': ['S5', 'S6'], 'name': ['Eva', 'Frank'], 'marks': [88, 92] }

df1 = pd.DataFrame(student_data1) 
df2 = pd.DataFrame(student_data2)

combined_df = pd.concat([df1, df2], axis=0)

print(combined_df)
```

## Output
<img width="408" height="202" alt="image" src="https://github.com/user-attachments/assets/799371b2-ccd7-4d45-8cc4-075e15f93bf5" />

## Result
Thus To write a Python program using Pandas to join two DataFrames along rows (row-wise concatenation) and assign all data to a new DataFrame. Hence the code has been executed successfully.

------------------------------------------------------------------------------------------

