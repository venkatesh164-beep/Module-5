# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
class Details:
    def __init__(self):<br>
        self.__id="<No Id>"<br>
        self.__name="<No Name>"<br>
        self.__gender="<No Gender>"<br>
    def setData(self,id,name,gender):<br>
        self.__id=id<br>
        self.__name=name<br>
        self.__gender=gender<br>
    def showData(self):<br>
        print("Id: ",self.__id)<br>
        print("Name: ", self.__name)<br>
        print("Gender: ", self.__gender)<br>

class Employee(Details): #Inheritance<br>
    def __init__(self):<br>
        self.__company="<No Company>"<br>
        self.__dept="<No Dept>"<br>
    def setEmployee(self,id,name,gender,comp,dept):<br>
        self.setData(id,name,gender)<br>
        self.__company=comp<br>
        self.__dept=dept<br>
    def showEmployee(self):<br>
        self.showData()<br>
        print("Hospital: ", self.__company)<br>
        print("Department: ", self.__dept)<br>

class Patient(Details): #Inheritance<br>
    def __init__(self):<br>
        self.__hospital="<No Hospital>"<br>
        self.__dept="<No Dept>"<br>
    def setEmployee(self,id,name,gender,hos,dept):<br>
        self.setData(id,name,gender)<br>
        self.__hospital=hos<br>
        self.__dept=dept<br>
    def showEmployee(self):<br>
        self.showData()<br>
        print("Hospital: ", self.__hospital)<br>
        print("Department: ", self.__dept)<br>

id=int(input())<br>
name=input()<br>
gender=input()<br>
comp=input()<br>
dept=input()<br>
id1=int(input())<br>
nam=input()<br>
gen=input()<br>
hosp=input()<br>
dep=input()<br>

print("Doctor Object")<br>
e=Employee()<br>
e.setEmployee(id,name,gender,comp,dept)<br>
e.showEmployee()<br>
print("\nPatient Object")<br>
d = Patient()<br>
d.setEmployee(id1, nam, gen, hosp, dep)<br>
d.showEmployee()
## Sample Output
<img width="1257" height="529" alt="image" src="https://github.com/user-attachments/assets/9e4d6031-e9ea-4278-8261-392ccd2f3f05" />

## Result


Thus the program that uses Hierarchical Inheritance to input and display Employee and Patient details hase been executed successfully.

