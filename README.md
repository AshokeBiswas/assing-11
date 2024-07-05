Q1. Explain Class and Object with respect to Object-Oriented Programming. Give a suitable example.
In object-oriented programming (OOP), a class is a blueprint or template for creating objects. It defines the properties (attributes) and behaviors (methods) that all objects of that class will have. An object is an instance of a class, representing a specific entity.
Example:
python
Copy code
# Define a class
class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model
    
    def display_info(self):
        print(f"{self.brand} {self.model}")

# Create objects (instances) of the class Car
car1 = Car("Toyota", "Camry")
car2 = Car("Honda", "Accord")

# Access attributes and call methods of objects
car1.display_info()  # Output: Toyota Camry
car2.display_info()  # Output: Honda Accord
In this example:
•	Car is a class that defines a blueprint for cars with attributes (brand, model) and methods (display_info()).
•	car1 and car2 are objects (instances) of the Car class, each representing a specific car with its own brand and model.
•	Objects encapsulate data (attributes) and behavior (methods) based on the class they belong to.
Q2. Name the four pillars of OOPs.
The four pillars of object-oriented programming (OOP) are:
1.	Encapsulation: Bundling data (attributes) and methods (functions) that operate on the data, hiding the internal state of an object from the outside world.
2.	Abstraction: Representing essential features without including background details.
3.	Inheritance: Allowing classes to inherit attributes and methods from other classes, promoting code reusability.
4.	Polymorphism: The ability to use a single interface for different data types or objects, enabling flexibility and extensibility in programming.
Q3. Explain why the __init__() function is used. Give a suitable example.
The __init__() function in Python is a constructor method used to initialize objects of a class. It is automatically called when an instance (object) of the class is created. It sets initial values for the object's attributes.
Example:
python
Copy code
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

# Creating an instance of Person
person1 = Person("Alice", 30)
In this example, __init__() initializes name and age attributes when person1 object is created
Q4. Why self is used in OOPs?
In object-oriented programming (OOP) in Python, self is used to refer to the instance of the class itself. It allows methods to access and modify attributes of the object they belong to. This ensures that each instance can maintain its own state separate from other instances of the same class.
Q5. What is inheritance? Give an example for each type of inheritance.
Inheritance in OOP allows one class (subclass/derived class) to inherit attributes and methods from another class (superclass/base class). Types include:
1.	Single Inheritance: One subclass inherits from one superclass.
python
Copy code
class Animal:
    def breathe(self):
        print("Breathing")

class Dog(Animal):
    def bark(self):
        print("Barking")
2.	Multiple Inheritance: One subclass inherits from multiple superclasses.
python
Copy code
class A:
    pass

class B:
    pass

class C(A, B):
    pass
3.	Multilevel Inheritance: One subclass inherits from another subclass.
python
Copy code
class A:
    pass

class B(A):
    pass

class C(B):
    pass
4.	Hierarchical Inheritance: Multiple subclasses inherit from one superclass.
python
Copy code
class Animal:
    pass

class Dog(Animal):
    pass

class Cat(Animal):
    pass

