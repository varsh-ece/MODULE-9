# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## 📌 Aim

To write a Python program that prints only the diagonal elements of a given matrix.

## 🧠 Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

## 🖥️ Program
```
rows = int(input("Enter the number of rows: "))
cols = int(input("Enter the number of columns: "))
matrix = []
print("Enter the matrix elements row-wise:")
for i in range(rows):
    row = list(map(int, input(f"Enter elements for row {i + 1} (space-separated): ").split()))
    matrix.append(row)
print("\nFull Matrix:")
for row in matrix:
    print(row)
print("\nDiagonal Elements:")
for i in range(rows):
    for j in range(cols):
        if i == j:
            print(matrix[i][j], end=" ")
        else:
            print(" ", end=" ")
    print()
```

### Output:
```
Enter the number of rows: 3
Enter the number of columns: 3
Enter the matrix elements row-wise:
Enter elements for row 1 (space-separated): 1 2 3
Enter elements for row 2 (space-separated): 4 5 6
Enter elements for row 3 (space-separated): 7 8 9

Full Matrix:
[1, 2, 3]
[4, 5, 6]
[7, 8, 9]

Diagonal Elements:
1    
  5  
    9
```
## Result
Hence Printd only the diagonal elements of a given matrix
