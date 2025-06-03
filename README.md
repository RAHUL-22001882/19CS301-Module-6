# 19CS301-Module-6
EX: 6a   POLYMORPHISM

### AIM: 
To Create two classes Employee and Admin. These two different classes have the same method name info(). This method contains information(name, department) about employee in Employee class and admin in Admin class.after initializing classes, Create two objects for respective classes. Then the method info() is called. Once by the object of Employee class and once by the object of Admin class.


### ALGORITHM:
Step1: create class Beans and def a function type and color

Step 2: create a class employee and admin

Step3: def a function info

Step 4: call the objects and execute the program

### PROGRAM:
```
class Employee:
    def info(self):
        #Add your code Here
        print('Rooney from Electronics')

class Admin:
    def info(self):
        #Add your code here
        print('Kalesh from CS')
        
        
obj_emp = Employee()
obj_adm = Admin()
for x in (obj_emp,obj_adm):
    x.info()
```
### OUTPUT:
![Screenshot 2025-06-02 120547](https://github.com/user-attachments/assets/e5374b27-4aa7-41ff-9878-b282d459f0a3)

### RESULT: Thus, the program has been successfully executed.

EXP.No: 6.b OPERATOR OVERLOADING

### AIM: write a python program to overload less than operator
###ALGORITHM:
Step1 :create class A and def init	 

Step2: def it	with a condition if self.a < o.a 

Step 3: call the function and execute the program.
### PROGRAM:
```
class A :
     def     init (self,a):
             self.a=a
     def     lt (self,o):
              if self.a < o.a :
                   return "ob1 is less than ob2"
              else:
                   return "ob2 is less than ob1"
ob1 = A(2)
ob2 = A(3)
print(ob1<ob2)
```

### OUTPUT:
![Screenshot 2025-06-02 121831](https://github.com/user-attachments/assets/706cf43f-0e63-4cac-8088-ca99a3a866a3)


### RESULT: Thus, the program has been successfully executed.

EX: 6.3 ABSTRACT CLASS METHOD

### AIM: To Create the abstract method calculate_area which is of the abstract class 'Shape'

### ALGORITHM:
Step1:Get input from the user

Step2:put class function to define the function using self

Step3:By using the function to find the area of the rectangle and circle Step4:Execute the program.

### PROGRAM:
```
from abc import ABC
class Shape(ABC): 
    def calculate_area(self):
        pass

class Rectangle(Shape):
  length = 6
  breadth = 4
  def calculate_area(self):
    return self.length * self.breadth

class Circle(Shape):
  radius = 7
  def calculate_area(self):
      return 3.14 * self.radius * self.radius

class Square(Shape):
  length = 4
  def calculate_area(self):
        return self.length * self.length
class triangle(Shape):
  length = 5
  width = 4
  def calculate_area(self):
      return 1/2 * self.length * self.width
r = Rectangle() 
c = Circle()
s = Square() 
t = triangle() 
print("Area of a rectangle:", r.calculate_area()) 
print("Area of a circle:", c.calculate_area()) 
print("Area of a square:", s.calculate_area())
print("Area of a triangle:", t.calculate_area())
```

### OUTPUT:
![Screenshot 2025-06-02 120659](https://github.com/user-attachments/assets/660f05b5-59ed-4134-95e9-7fc5455862b7)



### RESULT: Thus, the program has been successfully executed.

EXP.No: 6d     ENCAPSULATION
### AIM: 
To Implement Encapsulation using private members Use Name Mangling obj._ABC__fun() and obj._ABC__a concepts to access the private variables in ABC class.
### ALGORITHM: 
Start the program.

1.Define a class ABC.

2.In the init() constructor:

3.Declare a private instance variable __a and assign it the value 5.

4.Define a public method fun() that prints "I am public class method".

5.Define another method fun1():

6.Print "I am private class method".

7.Access and print the private variable __a.

8.Create an object x of class ABC.

9.Call the method x.fun() to execute the public method.

10.Call the method x.fun1() to execute the method that accesses the private variable.

End the program
### PROGRAM:
```
class ABC:
   def __init__(self):
       self.__a=5
   def fun(self):
       print("I am public class method")
   def fun1(self):
       print("I am private class method")
       print(self.__a)
x=ABC()
x.fun()
x.fun1()
```
### OUTPUT:
 
![Screenshot 2025-06-02 121201](https://github.com/user-attachments/assets/7a9c39a9-a03d-4067-ac6f-798406d66ddc)


### RESULT: Thus, the program has been successfully executed

EXP.No: 6e ENCAPSULATION-PUBLIC MEMBERS

### AIM:
Create a class Employee with public method show to display the details of the employee.

### ALGORITHM:
Start

Initialize the Employee Object:

m = Employee() creates an instance of the Employee class.

The constructor sets __price to 10000.

Display Salary (Initial Value):

Call m.sell() which prints Name: Jessa Salary: 10000.

Update Salary:

Call m.set(10000) to set the salary to 10000.

Display Salary (Updated Value):

Call m.sell() again, which prints the updated salary, which is still 10000.

End

### PROGRAM:
```
class Employee:
    def __init__(self):
        self.__price=10000
    def sell(self):
        print(f"Name:  Jessa Salary: {self.__price}")
    def set(self,x):
        self.__price=x
m=Employee()
m.sell()
m.set(10000)
m.sell()
```
### OUTPUT : 
![Screenshot 2025-06-02 122237](https://github.com/user-attachments/assets/4864fea3-5869-468d-9051-7e3cb4bbd89e)

### RESULT: 
Thus, the program has been successfully executed.



