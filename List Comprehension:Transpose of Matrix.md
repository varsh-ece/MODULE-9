# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

## 💻 PROGRAM:
```
r = int(input("Enter the number of rows: "))
c = int(input("Enter the number of columns: "))
def create(r, c):
    print("Enter the matrix elements row-wise:")
    matrix = []
    for i in range(r):
        row = list(map(int, input(f"Enter elements for row {i+1} (space-separated): ").split()))
        matrix.append(row)
    return matrix
matrix = create(r, c)
transpose = [[matrix[j][i] for j in range(r)] for i in range(c)]
print("\nTransposed Matrix:")
for row in transpose:
    print(row)
```
## OUTPUT:
```
Enter the number of rows: 2
Enter the number of columns: 3
Enter the matrix elements row-wise:
Enter elements for row 1 (space-separated): 1 2 3
Enter elements for row 2 (space-separated): 4 5 6
```
## RESULT:
Hence Computed the transpose of a matrix using list comprehension
