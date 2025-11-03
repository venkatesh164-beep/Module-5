# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
class Calculation1:<br>
    def Summation(self, a, b):<br>
        return a + b<br>

class Calculation2:<br>
    def Subtraction(self, a, b):<br>
        return a - b<br>

class Derived(Calculation1, Calculation2):<br>
    def Division(self, a, b):<br>
        if b != 0:<br>
            return a / b<br>
        else:<br>
            return "Error: Division by zero"<br>

a = int(input())<br>
b = int(input())<br>
obj = Derived()<br>

print(obj.Summation(a, b))<br>
print(obj.Subtraction(a, b))<br>
print(obj.Division(a, b))


## Output Example
<img width="1259" height="246" alt="image" src="https://github.com/user-attachments/assets/e386c8ab-f696-44d2-b3ec-501a8841370b" />

## Result
Thus the program demonstrates multiple inheritance by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes has been executed successfully.

