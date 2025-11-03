# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
class Parent:<br>
   def __init__(self,name):<br>
     self.name = name<br>
   def getName(self):<br>
     return self.name<br>

class Child(Parent):<br>
   def __init__(self,name,age):<br>
     Parent.__init__(self,name)<br>
     self.age = age<br>
   def getAge(self):<br>
     return self.age<br>

class Grandchild(Child):<br>
   def __init__(self,name,age,location):<br>
     Child.__init__(self,name,age)<br>
     self.location=location<br>
   def getLocation(self):<br>
     return self.location<br>

name=input()<br>
age=int(input())<br>
loc=input()<br>
gc = Grandchild(name,age,loc)<br>
print(gc.getName(), gc.getAge(), gc.getLocation())

## Sample Output
<img width="1255" height="244" alt="image" src="https://github.com/user-attachments/assets/50e3d949-95ec-4c05-b6fe-b31cfd6b3d46" />

 ## Result
 Thus the program that uses multilevel inheritance to get and display a person’s name, age, and location executed successfully.

