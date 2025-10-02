# # ➖ Matrix Operations-Matrix Subtraction in Python

## 🎯 AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` for rows and columns
3. Get the values of `r` and `c` from the user
4. Define a function `create_matrix(n, m)` to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the `create_matrix()` function twice to read two matrices `A` and `B`
6. Define a loop to subtract the elements of matrix `B` from matrix `A`
7. Store the result in a new matrix `C`
8. Print the resulting matrix `C`
9. **Stop**

---

## 💻 PROGRAM:
```
r = int(input("Enter the number of rows: "))
c = int(input("Enter the number of columns: "))
def create_matrix(n, m, name):
    print(f"Enter elements for Matrix {name}:")
    matrix = []
    for i in range(n):
        row = list(map(int, input(f"Enter row {i + 1} (space-separated): ").split()))
        if len(row) != m:
            print("Invalid number of columns. Please re-enter the row.")
            return create_matrix(n, m, name)
        matrix.append(row)
    return matrix

A = create_matrix(r, c, 'A')
B = create_matrix(r, c, 'B')
C = []
for i in range(r):
    row = []
    for j in range(c):
        row.append(A[i][j] - B[i][j])
    C.append(row)
print("\nResultant Matrix C (A - B):")
for row in C:
    print(row)
```
## OUTPUT:
```
Enter the number of rows: 2
Enter the number of columns: 2
Enter elements for Matrix A:
Enter row 1 (space-separated): 5 8
Enter row 2 (space-separated): 7 6
Enter elements for Matrix B:
Enter row 1 (space-separated): 3 2
Enter row 2 (space-separated): 4 5

Resultant Matrix C (A - B):
[2, 6]
[3, 1]
```
## RESULT:
Hence Matrix Subtraction of Two User-Input Matrices is done.
