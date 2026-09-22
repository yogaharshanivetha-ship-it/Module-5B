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
```
import pandas as pd

student_data1 = {
    'student_id': [1, 2, 3],
    'name': ['Alice', 'Bob', 'Charlie'],
    'score': [85, 90, 95]
}

student_data2 = {
    'student_id': [4, 5, 6],
    'name': ['David', 'Eva', 'Frank'],
    'score': [88, 92, 97]
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

result = pd.concat([df1, df2], axis=0)

print(result)
```

## Output
<img width="1270" height="497" alt="image" src="https://github.com/user-attachments/assets/3e71f037-39e0-4ec4-aae5-dbdbf8340e22" />

## Result
The program creates two Pandas DataFrames using dictionaries, concatenates them row-wise using pd.concat(..., axis=0), and displays the combined DataFrame.
