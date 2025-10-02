# 🧾 List Comprehension:Generates all even numbers between 200 and 300
## 🎯 AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

## 💻 PROGRAM:
```
class Program:
    def __init__(self):
        self.a = 200  # Lower limit
        self.b = 2    # Step value
        self.c = 300  # Upper limit

    def display(self):
        even_numbers = [i for i in range(self.a, self.c + 1, self.b) if i % 2 == 0]
        print("Even numbers between 200 and 300:")
        print(even_numbers)
obj = Program()
obj.display()
```

## OUTPUT:
```
Even numbers between 200 and 300:
[200, 202, 204, ..., 298, 300]
```
## RESULT:
Hence Generated even numbers between 200 and 300 using list comprehension in a class
