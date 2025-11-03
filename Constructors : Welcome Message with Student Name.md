# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
class Student:<br>
    def _init_(self,a):<br>
        self.a=a<br>
    def get(self):<br>
        self.a=input()<br>
    def info(self):<br>
        print("This is non parametrized constructor")<br>
        print("Hello",self.a)<br>
obj=Student()<br>
obj.get()<br>
obj.info()

## Output
<img width="1258" height="366" alt="image" src="https://github.com/user-attachments/assets/c0b88226-64f9-4ac8-8bfb-72f742f3f838" />

## Result
Thus the program demonstrates how to implement a destructor in Python using a simple class has been executed successfully.
