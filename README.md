# Class-and-Objects
```markdown
# Experiment_11

## Contents
- Aim
- Software Used
- Theory
  - Definition
  - Class
  - Object
  - OOP Principles
  - Advantages
- Algorithms
- Conclusion

---

## Aim
To study Class and Objects

---

## Software Used
- VS Code
- Dev C++

---

## Theory

### Definition
Object-Oriented Programming (OOP) is a programming principle centered around the concept of "objects."

### What is a Class?
A class is basically a framework or blueprint which we use to create objects. It encapsulates data and functions that operate on the data. Objects share similarities with their class. For example, children and their parents, where children could be considered objects of the parent class.

For example:

```cpp
#include <iostream>
using namespace std;

class Dog {
public:
    string name;
    int age;

    void bark() {
        cout << name << " Woof!" << endl;
    }
};
```

### What is an Object?
An object is an instance of a class. It is a self-contained unit that contains both data and methods. The data (attributes) represents the state of the object, while the methods (functions) define its behavior. For example, in a class `Car`, an object could be a specific car with features like color and model, and operations like starting the engine, driving.

An object has two defining features:

- **Attributes**: Properties of an object, representing its characteristics (e.g., a `Car` object might have attributes like color, model, year).
  
- **Methods**: Functions or behaviors that an object can perform (e.g., methods like `start_engine()`, `drive()` for a `Car` object).

For Example: Creating an object of class `Dog`:

```cpp
int main() {
    Dog myDog;
    myDog.name = "Buddy";
    myDog.age = 3;

    myDog.bark();

    return 0;
}
```

---

## Principles of OOP in C++

1. **Encapsulation**  
   Encapsulation is the concept of bundling data and methods that operate on that data within a single unit, typically a class. It hides the internal state of the object from the outside world and only exposes a controlled interface.

   Example: In C++, encapsulation is achieved using classes. Data members (attributes) are kept private or protected, and access to these members is provided through public methods (getters and setters).

2. **Inheritance**  
   Inheritance allows a class (derived class) to inherit properties and behaviors (methods) from another class (base class). This promotes code reusability and establishes a hierarchy between classes.

   ```cpp
   class Animal {
   public:
       void eat() { std::cout << "Eating..." << std::endl; }
   };

   class Dog : public Animal {
   public:
       void bark() { std::cout << "Barking..." << std::endl; }
   };
   ```

3. **Polymorphism**  
   Polymorphism allows objects of different classes to be treated as objects of a common base class. The most common use of polymorphism is to call methods on objects of derived classes through base class pointers or references, enabling dynamic method binding.

4. **Abstraction**  
   Abstraction focuses on hiding the complex implementation details and showing only the necessary features of an object. It simplifies interactions with objects by exposing only the relevant methods and properties.

---

## Advantages of Using Classes and Objects

- **Modularity**: Classes and objects promote modularity in programming by dividing a program into distinct, manageable sections. Each class represents a specific component or concept.
  
- **Reusability**: Classes allow code reuse through inheritance and composition, reducing duplication and effort.
  
- **Maintainability**: Encapsulation makes code easier to maintain. Changes to a class automatically reflect in all its objects.
  
- **Scalability**: Object-oriented design supports scalability by allowing new classes and methods to be added without affecting existing code.
  
- **Real-World Modeling**: Classes and objects align closely with real-world concepts and entities, making it easier to model complex systems.

---

## Algorithms

### Algorithm for defining a class:

1. **Start**
2. Define a class named `Student`:
   - Declare public member variables:
     - `string name`
     - `int age`
     - `string branch`
     - `float result`
     - `string year`
3. In `main()` function:
   - Create an object `student1` of type `Student`.
   - Set attributes for `student1`.
   - Print the details of `student1`.
4. **End**

---

### Algorithm for defining a method inside a class:

1. **Start**
2. Define a class `Student`:
   - Attributes:
     - `string name`
     - `int age`
     - `string branch`
     - `float result`
     - `string year`
3. Define a method `void printYear()` to print the year of study.
4. In `main()` function:
   - Create and initialize a `Student` object `student1`.
   - Print student details and call `printYear()` to display the year.
5. **End**

---

### Algorithm for defining a method outside a class:

1. **Start**
2. Define class `Student`:
   - Attributes:
     - `string name`
     - `int age`
     - `string branch`
     - `float result`
     - `string year`
3. Define method `void printYear()` outside the class.
4. In `main()` function:
   - Create and initialize a `Student` object `student1`.
   - Print student details and call `printYear()` to display the year.
5. **End**

---

### Algorithm for calculating the volume of a cuboid:

1. **Start**
2. Define class `Cuboid`:
   - Attributes:
     - `float length`
     - `float breadth`
     - `float height`
     - `float volume`
3. Methods:
   - `void inputDimensions()` to input cuboid dimensions.
   - `void calculateVolume()` to compute the volume.
   - `void displayVolume()` to display the volume.
4. In `main()` function:
   - Create an object `cuboid` of type `Cuboid`.
   - Call methods to input dimensions, calculate, and display the volume.
5. **End**

---

## Conclusion
We learned how to use the concepts of Class and Objects in programming.
