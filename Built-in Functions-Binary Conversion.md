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
print(bin(a))
```

## Output

<img width="562" height="265" alt="image" src="https://github.com/user-attachments/assets/bc93c40a-488e-4fc2-89b7-6efaff57c457" />

## Result

Thus, the program has been successfully executed.


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
def result(a, b):
    modulo_value = a % b
    return modulo_value

a=int(input())
b=int(input())
print("modulo is", result(a, b))
```

## Output

<img width="662" height="311" alt="image" src="https://github.com/user-attachments/assets/27cff632-6d6c-4b9a-bad7-3984329c8ec6" />

## Result

The program to return two values modulo is successful.

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
def factorial(n):
    if n == 0 or n == 1:
        return 1
    return n * factorial(n - 1)

def combination(n, k):
    return factorial(n) // (factorial(k) * factorial(n - k))

num_rows = int(input("Enter number of rows: "))

for i in range(num_rows):
    print(' ' * (num_rows - i - 1), end='')
    for j in range(i + 1):
        print(combination(i, j), end=' ')
    print()
```

## Sample Output

<img width="201" height="225" alt="image" src="https://github.com/user-attachments/assets/0981e0cf-d655-4137-896b-312886c53fc3" />

## Result

Thus, the program has been successfully executed

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
``` python
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

<img width="593" height="114" alt="image" src="https://github.com/user-attachments/assets/fbc45cbf-8cf2-47de-947f-58a2e7d476f2" />

## Result

Thus, the program has been successfully executed .
