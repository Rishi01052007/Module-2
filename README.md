# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program
```python
a=16
print("The binary representation for sixteen is")
print(bin(a))
```

## Output
![Screenshot 2025-04-29 225012](https://github.com/user-attachments/assets/c9aacbe6-5f3e-4a01-a5a2-8b5e1dad5095)

## Result
Hence the program executed successfully!
# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program
```python
def result(a,b):
    c=a%b
    return c
a=int(input())
b=int(input())
print(f"modulo is {result(a,b)}")
```

## Output
![Screenshot 2025-04-29 225308](https://github.com/user-attachments/assets/7597c929-92cf-4646-a4b8-33cf3ced29f5)


## Result
Hence the program executed successfully!
# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
```python
a=int(input("Enter a 1st digit :"))
b=int(input("Enter a 2nd digit :"))
f = lambda a, b: a+b
print(f(a,b))
```

## Output
![Screenshot 2025-04-29 225818](https://github.com/user-attachments/assets/168da22a-6b3d-4bd6-ac3d-594b6b91a32d)


## Result
Hence the program executed successfully!
# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```python
 rows = int(input())
coef = 1

for i in range(1, rows+1):
    for space in range(1, rows-i+1):
        print(" ",end="")
    for j in range(0, i):
        if j==0 or i==0:
            coef = 1
        else:
            coef = coef * (i - j)//j
        print(coef, end = " ")
    print()
```

## Sample Output
![Screenshot 2025-04-29 230019](https://github.com/user-attachments/assets/1068da67-cd7f-4b9d-87df-47ca4b2872e8)


## Result
Hence the program executed successfully!


## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```python
num=int(input())
rev=0
temp=num
while temp>0:
    rev=(10*rev)+temp%10
    temp//=10
if rev==num:
    print("The given number {} is a Palindrome".format(num))
else:
    print("The given number {} is not a palindrome".format(num))
```
## Output
![Screenshot 2025-04-29 230236](https://github.com/user-attachments/assets/6294b1fa-2a77-4001-8caf-e355885e1b09)


## Result
Hence the program executed successfully!
