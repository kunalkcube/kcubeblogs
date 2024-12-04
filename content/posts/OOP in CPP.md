---
title: OOP in CPP
date: 2024-12-03
draft: false
tags:
  - cpp
  - programming
  - oop
---

## **Unit 1: Introduction to Object-Oriented Programming (OOP)**

## **Basic Concepts of Object-Oriented Programming**

### **Definition**

Object-Oriented Programming (OOP) is a programming paradigm that organizes software design around **objects** rather than functions and logic. Objects are instances of classes that encapsulate data and behavior.
<!--more-->

### **Key Concepts**

1. **Class**: A blueprint for creating objects (data structures).
2. **Object**: An instance of a class containing data and methods.
3. **Encapsulation**: Wrapping data and methods into a single unit (class).
4. **Inheritance**: A mechanism for creating a new class from an existing class.
5. **Polymorphism**: The ability to process objects differently based on their data type or class.
6. **Abstraction**: Hiding internal details and showing only the essential features.

---

### **Benefits of OOP**

1. **Modularity**: Code is divided into smaller, reusable units (classes).
2. **Reusability**: Classes and objects can be reused in other programs.
3. **Scalability**: Easy to scale and maintain applications.
4. **Data Security**: Encapsulation helps protect data from unauthorized access.
5. **Real-World Modeling**: OOP mimics real-world systems effectively.

---

### **Applications of OOP**

- **Game Development**: E.g., characters (objects) with unique properties (attributes) and actions (methods).
- **GUI Applications**: E.g., buttons and windows as objects in a graphical user interface.
- **Database Management**: Representing tables as classes.
- **Web Development**: Frameworks like Django (Python) and Spring (Java) use OOP principles.

---

## **Object-Oriented Design (OOD)**

### **Definition**

Object-Oriented Design is the process of planning a system of interacting objects to solve a software problem. It emphasizes designing reusable and maintainable classes.

### **Principles of OOD**

1. **SOLID Principles**:
    - **S**ingle Responsibility
    - **O**pen/Closed
    - **L**iskov Substitution
    - **I**nterface Segregation
    - **D**ependency Inversion
2. **DRY Principle**: Don’t Repeat Yourself.
3. **KISS Principle**: Keep It Simple, Stupid.
4. **Encapsulation**: Protect data by restricting direct access.
5. **Separation of Concerns**: Divide application into distinct features.

---

### **Example Program: Simple OOP Concept in C++**

```cpp
#include <iostream>
using namespace std;

// Class definition
class Car {
private:
    string brand;
    int speed;

public:
    // Constructor
    Car(string b, int s) {
        brand = b;
        speed = s;
    }

    // Method to display car details
    void displayDetails() {
        cout << "Brand: " << brand << ", Speed: " << speed << " km/h" << endl;
    }
};

int main() {
    // Creating objects
    Car car1("Toyota", 180);
    Car car2("BMW", 240);

    // Displaying details
    car1.displayDetails();
    car2.displayDetails();

    return 0;
}
```

---

## **Comparison of Procedural Programming and Object-Oriented Programming**

|Feature|Procedural Programming|Object-Oriented Programming|
|---|---|---|
|**Approach**|Focuses on functions and logic.|Focuses on objects and their interactions.|
|**Data Security**|Less secure; data is globally accessible.|Highly secure; data is encapsulated.|
|**Reusability**|Limited reusability.|High reusability through classes.|
|**Real-World Modeling**|Difficult to model real-world systems.|Mimics real-world systems effectively.|
|**Examples**|C, Pascal, Fortran|C++, Java, Python|

---

### **Example Program: Procedural vs Object-Oriented**

#### **Procedural Approach**

```cpp
#include <iostream>
using namespace std;

void displayCar(string brand, int speed) {
    cout << "Brand: " << brand << ", Speed: " << speed << " km/h" << endl;
}

int main() {
    displayCar("Toyota", 180);
    displayCar("BMW", 240);
    return 0;
}
```

#### **Object-Oriented Approach**

```cpp
#include <iostream>
using namespace std;

class Car {
private:
    string brand;
    int speed;

public:
    Car(string b, int s) : brand(b), speed(s) {}

    void displayDetails() {
        cout << "Brand: " << brand << ", Speed: " << speed << " km/h" << endl;
    }
};

int main() {
    Car car1("Toyota", 180);
    Car car2("BMW", 240);

    car1.displayDetails();
    car2.displayDetails();

    return 0;
}
```



---


## **Unit 2: Introduction to C++**

## **Structure of a Simple C++ Program**

### **Basic Structure**

1. **Preprocessor Directives**: Includes necessary libraries (`#include`).
2. **Namespace**: Defines the scope for standard library functions (e.g., `std`).
3. **Main Function**: Entry point of the program (`int main()`).
4. **Body**: Contains statements and logic.
5. **Return Statement**: Indicates program termination (`return 0;`).

### **Example**

```cpp
#include <iostream> // Preprocessor directive
using namespace std; // Namespace

int main() { // Main function
    cout << "Hello, World!"; // Output statement
    return 0; // Program ends
}
```

---

## **Input and Output Operators**

### **Output Operator (`<<`)**

Used to send data to the output stream (e.g., `cout`).

```cpp
cout << "Hello, World!";
```

### **Input Operator (`>>`)**

Used to receive data from the input stream (e.g., `cin`).

```cpp
int num;
cin >> num; // Accepts user input
```

### **Cascading of I/O Operators**

Allows chaining of multiple input/output operations.

```cpp
cout << "Enter two numbers: ";
int a, b;
cin >> a >> b; // Accepts two inputs
cout << "Sum: " << a + b << endl;
```

---

## **Tokens in C++**

### **Definition**

Tokens are the smallest building blocks of a C++ program.

### **Types of Tokens**

1. **Keywords**: Reserved words (e.g., `int`, `float`, `if`).
2. **Identifiers**: Names for variables, functions, etc.
3. **Constants**: Fixed values (e.g., `3.14`, `"Hello"`).
4. **Strings**: Text enclosed in double quotes (e.g., `"Welcome"`).
5. **Operators**: Symbols for operations (e.g., `+`, `-`).

---

## **Data Types**

### **Basic Data Types**

|**Data Type**|**Size**|**Range**|
|---|---|---|
|`int`|4 bytes|-2,147,483,648 to 2,147,483,647|
|`float`|4 bytes|±3.4e-38 to ±3.4e+38|
|`char`|1 byte|-128 to 127|
|`bool`|1 byte|`true` or `false`|

### **User-Defined Data Types**

Defined by the programmer (e.g., `struct`, `class`).

### **Dynamic Initialization of Variables**

Allows initializing variables at runtime using expressions.

```cpp
int x = 5, y = 10;
int sum = x + y; // Dynamically initialized
```

---

## **Reference Variables**

### **Definition**

A reference is an alias for an already existing variable.

### **Syntax**

```cpp
int a = 10;
int &ref = a; // 'ref' is a reference to 'a'
```

### **Example**

```cpp
#include <iostream>
using namespace std;

int main() {
    int x = 10;
    int &y = x; // Reference variable
    cout << "x: " << x << ", y: " << y << endl;
    y = 20; // Modifies 'x' through 'y'
    cout << "x: " << x << ", y: " << y << endl;
    return 0;
}
```

---

## **Operators in C++**

### **Scope Resolution Operator (`::`)**

Used to access global variables or class members.

```cpp
#include <iostream>
using namespace std;

int x = 10; // Global variable

int main() {
    int x = 20; // Local variable
    cout << "Local x: " << x << endl;
    cout << "Global x: " << ::x << endl; // Access global variable
    return 0;
}
```

### **Member Dereferencing Operators**

- **`.`**: Access members of an object.
- **`->`**: Access members of a pointer to an object.

---

## **Memory Management Operators**

### **Definition**

- `new`: Allocates memory dynamically.
- `delete`: Deallocates memory dynamically.

### **Example**

```cpp
#include <iostream>
using namespace std;

int main() {
    int *ptr = new int(5); // Dynamic memory allocation
    cout << "Value: " << *ptr << endl;
    delete ptr; // Free memory
    return 0;
}
```

---

## **Control Structures**

### **Simple `if`**

```cpp
int x = 10;
if (x > 5) {
    cout << "x is greater than 5";
}
```

### **`if-else`**

```cpp
int x = 10;
if (x > 5) {
    cout << "x is greater than 5";
} else {
    cout << "x is not greater than 5";
}
```

### **`switch`**

```cpp
int choice = 2;
switch (choice) {
    case 1: cout << "Choice is 1"; break;
    case 2: cout << "Choice is 2"; break;
    default: cout << "Invalid choice"; break;
}
```

---

## **Introduction to Functions**

### **Function Prototyping**

Defines the function signature.

```cpp
int add(int, int); // Prototype
```

### **Call-by-Reference**

```cpp
void swap(int &a, int &b) {
    int temp = a;
    a = b;
    b = temp;
}
```

### **Inline Functions**

Improves performance by replacing function calls with code.

```cpp
inline int square(int x) {
    return x * x;
}
```

### **Default Arguments**

```cpp
int add(int x, int y = 10) { // 'y' has a default value
    return x + y;
}
```

### **Const Arguments**

Prevents modification of arguments.

```cpp
void display(const int x) {
    cout << x;
}
```

---

## **Sample Program: Comprehensive Example**

```cpp
#include <iostream>
using namespace std;

// Function with default arguments
int multiply(int a, int b = 5) {
    return a * b;
}

// Function call-by-reference
void swap(int &x, int &y) {
    int temp = x;
    x = y;
    y = temp;
}

int main() {
    // Dynamic initialization
    int a = 10, b = 20;

    // Function call
    cout << "Product: " << multiply(a) << endl;

    // Call-by-reference
    cout << "Before swap: a = " << a << ", b = " << b << endl;
    swap(a, b);
    cout << "After swap: a = " << a << ", b = " << b << endl;

    return 0;
}
```



---


# **Unit 3: Classes and Objects**

## **Introduction to Classes and Objects**

### **Classes**

A class is a blueprint for creating objects. It defines properties (attributes) and behaviors (methods) that the objects created from the class can have.

### **Syntax**

```cpp
class ClassName {
public:
    int attribute;       // Attribute
    void method() {      // Method
        cout << "Method called!" << endl;
    }
};
```

### **Objects**

Objects are instances of classes. They can access attributes and methods defined in the class.

### **Example**

```cpp
#include <iostream>
using namespace std;

class Car {
public:
    string brand;
    int year;

    void display() {
        cout << "Brand: " << brand << ", Year: " << year << endl;
    }
};

int main() {
    Car car1;
    car1.brand = "Toyota";
    car1.year = 2020;
    car1.display();

    return 0;
}
```

---

## **Class vs. Structure**

|**Aspect**|**Class**|**Structure**|
|---|---|---|
|**Default Access**|Private|Public|
|**Inheritance**|Supported|Not supported|
|**Functionality**|Can have member functions|Limited functionality|

---

## **Access Modifiers**

1. **Public**: Accessible from anywhere.
2. **Private**: Accessible only within the class.
3. **Protected**: Accessible within the class and derived classes.

### **Example**

```cpp
class Example {
private:
    int privateVar;

protected:
    int protectedVar;

public:
    int publicVar;
};
```

---

## **Defining Member Functions**

### **Inside the Class Definition**

Defined directly within the class body.

```cpp
class Example {
public:
    void display() {
        cout << "Inside the class!" << endl;
    }
};
```

### **Outside the Class Definition**

Defined outside the class using the scope resolution operator (`::`).

```cpp
class Example {
public:
    void display(); // Declaration
};

// Definition
void Example::display() {
    cout << "Outside the class!" << endl;
}
```

### **Inline Member Functions**

Small functions can be defined inline for faster execution.

```cpp
inline void greet() {
    cout << "Hello, World!" << endl;
}
```

---

## **Nesting of Member Functions**

One member function can call another within the same class.

```cpp
class Example {
public:
    void display() {
        show();
    }

private:
    void show() {
        cout << "Nested function called!" << endl;
    }
};
```

---

## **Memory Allocation for Objects**

Memory is allocated when an object is created. The size depends on the attributes and functions.

### **Example**

```cpp
#include <iostream>
using namespace std;

class Example {
    int a; // Memory allocated for attribute
public:
    void display() {
        cout << "Memory allocated for object!" << endl;
    }
};

int main() {
    Example obj; // Memory allocated
    obj.display();
    return 0;
}
```

---

## **Array of Objects**

### **Definition**

An array of objects allows storing multiple objects of the same class.

### **Example**

```cpp
#include <iostream>
using namespace std;

class Student {
public:
    string name;
    int age;

    void display() {
        cout << "Name: " << name << ", Age: " << age << endl;
    }
};

int main() {
    Student students[2];

    // Input
    students[0].name = "Alice";
    students[0].age = 20;

    students[1].name = "Bob";
    students[1].age = 22;

    // Output
    students[0].display();
    students[1].display();

    return 0;
}
```

---

## **Friendly Functions**

### **Definition**

A friend function is not a member of a class but can access its private and protected members.

### **Syntax**

Use the `friend` keyword to declare a friend function.

```cpp
class Example {
    int a;

public:
    Example(int x) : a(x) {}

    friend void display(Example); // Friend function
};

void display(Example obj) {
    cout << "Value: " << obj.a << endl;
}

int main() {
    Example obj(10);
    display(obj);
    return 0;
}
```

---

## **Comprehensive Program**

### **Combining Concepts**

```cpp
#include <iostream>
using namespace std;

class Employee {
private:
    int empId;
    float salary;

public:
    // Constructor
    Employee(int id, float sal) : empId(id), salary(sal) {}

    // Member function
    void display() const {
        cout << "Employee ID: " << empId << ", Salary: " << salary << endl;
    }

    // Friend function
    friend void updateSalary(Employee &e, float increment);
};

// Friend function definition
void updateSalary(Employee &e, float increment) {
    e.salary += increment;
}

int main() {
    Employee emp1(101, 50000);

    // Display details
    emp1.display();

    // Update salary using friend function
    updateSalary(emp1, 5000);

    // Display updated details
    emp1.display();

    return 0;
}
```

---

## **Constructors**

### **Definition**

A constructor is a special member function that is automatically called when an object is created. It is used to initialize the object.

### **Characteristics of Constructors**

- Must have the same name as the class.
- Cannot have a return type.
- Can be overloaded.

### **Types of Constructors**

1. **Default Constructor**: Takes no arguments.
2. **Parameterized Constructor**: Takes parameters to initialize data members.
3. **Constructor with Default Arguments**: Allows some or all arguments to have default values.
4. **Copy Constructor**: Creates a new object as a copy of an existing object.

---

### **Default Constructor**

A constructor with no arguments.  
**Example:**

```cpp
#include <iostream>
using namespace std;

class Example {
public:
    int value;

    Example() { // Default Constructor
        value = 0;
        cout << "Default Constructor called!" << endl;
    }

    void display() {
        cout << "Value: " << value << endl;
    }
};

int main() {
    Example obj;
    obj.display();
    return 0;
}
```

---

### **Parameterized Constructor**

A constructor with arguments to initialize the data members.  
**Example:**

```cpp
#include <iostream>
using namespace std;

class Rectangle {
    int length, width;

public:
    Rectangle(int l, int w) { // Parameterized Constructor
        length = l;
        width = w;
    }

    int area() {
        return length * width;
    }
};

int main() {
    Rectangle rect(10, 5);
    cout << "Area: " << rect.area() << endl;
    return 0;
}
```

---

### **Constructor with Default Arguments**

A constructor that uses default values if arguments are not provided.  
**Example:**

```cpp
#include <iostream>
using namespace std;

class Rectangle {
    int length, width;

public:
    Rectangle(int l = 1, int w = 1) { // Constructor with Default Arguments
        length = l;
        width = w;
    }

    int area() {
        return length * width;
    }
};

int main() {
    Rectangle rect1(10, 5); // Both arguments provided
    Rectangle rect2;        // Default arguments used
    cout << "Area 1: " << rect1.area() << endl;
    cout << "Area 2: " << rect2.area() << endl;
    return 0;
}
```

---

### **Copy Constructor**

A constructor that initializes an object using another object of the same class.  
**Example:**

```cpp
#include <iostream>
using namespace std;

class Example {
    int value;

public:
    Example(int v) { // Parameterized Constructor
        value = v;
    }

    Example(const Example &obj) { // Copy Constructor
        value = obj.value;
    }

    void display() {
        cout << "Value: " << value << endl;
    }
};

int main() {
    Example obj1(10);
    Example obj2 = obj1; // Copy Constructor called
    obj2.display();
    return 0;
}
```

---

### **Dynamic Initialization of Objects**

Objects can be initialized dynamically using constructors.  
**Example:**

```cpp
#include <iostream>
using namespace std;

class Example {
    int *ptr;

public:
    Example(int val) { // Dynamic Initialization
        ptr = new int(val);
    }

    void display() {
        cout << "Value: " << *ptr << endl;
    }

    ~Example() { // Destructor to free memory
        delete ptr;
        cout << "Memory freed!" << endl;
    }
};

int main() {
    Example obj(20);
    obj.display();
    return 0;
}
```

---

### **Dynamic Constructors and Destructors**

Used to allocate and deallocate memory dynamically.  
**Example:**

```cpp
#include <iostream>
using namespace std;

class Example {
    int *arr;
    int size;

public:
    Example(int s) { // Dynamic Constructor
        size = s;
        arr = new int[size];
    }

    ~Example() { // Dynamic Destructor
        delete[] arr;
        cout << "Memory released!" << endl;
    }
};

int main() {
    Example obj(5);
    return 0;
}
```

---

## **Destructors**

### **Definition**

A destructor is a special member function that is called automatically when an object goes out of scope or is deleted. It is used to release resources.

### **Characteristics**

- Same name as the class prefixed with `~`.
- No return type.
- Cannot be overloaded.

**Example:**

```cpp
#include <iostream>
using namespace std;

class Example {
public:
    Example() {
        cout << "Constructor called!" << endl;
    }

    ~Example() {
        cout << "Destructor called!" << endl;
    }
};

int main() {
    Example obj;
    return 0;
}
```



---


# **Unit 4: Function and Operator Overloading**

## **Concept of Overloading**

### **Definition**

Overloading allows defining multiple functions or operators with the same name but different behaviors based on the parameters or operands.

---

## **Function Overloading**

### **Definition**

Creating multiple functions with the same name but different parameter lists.

**Example:**

```cpp
#include <iostream>
using namespace std;

class Example {
public:
    void display() {
        cout << "No parameters" << endl;
    }

    void display(int x) {
        cout << "Integer parameter: " << x << endl;
    }

    void display(double y) {
        cout << "Double parameter: " << y << endl;
    }
};

int main() {
    Example obj;
    obj.display();
    obj.display(5);
    obj.display(5.5);
    return 0;
}
```

---

### **Default and Constant Parameters**

Default values and constant parameters can also be used in overloaded functions.

**Example:**

```cpp
#include <iostream>
using namespace std;

void greet(string name = "User") {
    cout << "Hello, " << name << "!" << endl;
}

int main() {
    greet();             // Default parameter used
    greet("Alice");      // Custom parameter passed
    return 0;
}
```

---

## **Operator Overloading**

### **Definition**

Allows redefining the behavior of operators for user-defined data types.

---

### **Overloading Unary Operators**

Unary operators like `++` or `--` can be overloaded.

**Example:**

```cpp
#include <iostream>
using namespace std;

class Counter {
    int count;

public:
    Counter(int c) : count(c) {}

    void operator++() { // Overloading prefix ++
        ++count;
    }

    void display() {
        cout << "Count: " << count << endl;
    }
};

int main() {
    Counter c(10);
    ++c; // Calls overloaded operator++
    c.display();
    return 0;
}
```

---

### **Overloading Binary Operators**

Binary operators like `+` can be overloaded.

**Example:**

```cpp
#include <iostream>
using namespace std;

class Complex {
    int real, imag;

public:
    Complex(int r, int i) : real(r), imag(i) {}

    Complex operator+(const Complex &c) { // Overloading +
        return Complex(real + c.real, imag + c.imag);
    }

    void display() {
        cout << real << " + " << imag << "i" << endl;
    }
};

int main() {
    Complex c1(1, 2), c2(3, 4);
    Complex c3 = c1 + c2; // Calls overloaded operator+
    c3.display();
    return 0;
}
```

---

### **Overloading Using Friend Functions**

**Example:**

```cpp
#include <iostream>
using namespace std;

class Complex {
    int real, imag;

public:
    Complex(int r, int i) : real(r), imag(i) {}

    friend Complex operator+(const Complex &c1, const Complex &c2); // Friend function

    void display() {
        cout << real << " + " << imag << "i" << endl;
    }
};

Complex operator+(const Complex &c1, const Complex &c2) {
    return Complex(c1.real + c2.real, c1.imag + c2.imag);
}

int main() {
    Complex c1(1, 2), c2(3, 4);
    Complex c3 = c1 + c2; // Friend function used
    c3.display();
    return 0;
}
```



---


# **Unit 5: Inheritance and Polymorphism**

## **Concept of Inheritance**

Inheritance allows a class (derived class) to acquire properties and behaviors of another class (base class). This promotes code reuse and hierarchical relationships.

---

### **Defining Derived Classes**

A derived class is created using the `:` symbol followed by the access specifier and the base class name.

**Example:**

```cpp
#include <iostream>
using namespace std;

class Base {
public:
    void display() {
        cout << "Base class function" << endl;
    }
};

class Derived : public Base {
public:
    void show() {
        cout << "Derived class function" << endl;
    }
};

int main() {
    Derived obj;
    obj.display(); // Inherited function
    obj.show();
    return 0;
}
```

---

### **Types of Inheritance**

1. **Single Inheritance**: One derived class inherits from one base class.
2. **Multilevel Inheritance**: A class is derived from another derived class.
3. **Multiple Inheritance**: A class inherits from multiple base classes.
4. **Hierarchical Inheritance**: Multiple derived classes inherit from a single base class.
5. **Hybrid Inheritance**: Combination of two or more types of inheritance.

---

#### **1. Single Inheritance**

**Example:**

```cpp
#include <iostream>
using namespace std;

class Base {
public:
    void greet() {
        cout << "Hello from Base class!" << endl;
    }
};

class Derived : public Base {};

int main() {
    Derived obj;
    obj.greet(); // Accessing Base class method
    return 0;
}
```

---

#### **2. Multilevel Inheritance**

**Example:**

```cpp
#include <iostream>
using namespace std;

class Grandparent {
public:
    void message() {
        cout << "Grandparent class" << endl;
    }
};

class Parent : public Grandparent {};

class Child : public Parent {};

int main() {
    Child obj;
    obj.message(); // Inherited from Grandparent
    return 0;
}
```

---

#### **3. Multiple Inheritance**

**Example:**

```cpp
#include <iostream>
using namespace std;

class ClassA {
public:
    void displayA() {
        cout << "Class A function" << endl;
    }
};

class ClassB {
public:
    void displayB() {
        cout << "Class B function" << endl;
    }
};

class Derived : public ClassA, public ClassB {};

int main() {
    Derived obj;
    obj.displayA();
    obj.displayB();
    return 0;
}
```

---

#### **4. Hierarchical Inheritance**

**Example:**

```cpp
#include <iostream>
using namespace std;

class Base {
public:
    void greet() {
        cout << "Greetings from Base class!" << endl;
    }
};

class Derived1 : public Base {};
class Derived2 : public Base {};

int main() {
    Derived1 obj1;
    Derived2 obj2;
    obj1.greet();
    obj2.greet();
    return 0;
}
```

---

#### **5. Hybrid Inheritance**

**Example:**

```cpp
#include <iostream>
using namespace std;

class A {
public:
    void displayA() {
        cout << "Class A function" << endl;
    }
};

class B : public A {};
class C : public A {};
class D : public B, public C {};

int main() {
    D obj;
    obj.B::displayA(); // Resolving ambiguity
    return 0;
}
```

---

### **Virtual Base Classes**

Used to avoid duplication of base class properties in hybrid inheritance.

**Example:**

```cpp
#include <iostream>
using namespace std;

class Base {
public:
    void show() {
        cout << "Base class" << endl;
    }
};

class Derived1 : virtual public Base {};
class Derived2 : virtual public Base {};
class FinalDerived : public Derived1, public Derived2 {};

int main() {
    FinalDerived obj;
    obj.show(); // No ambiguity
    return 0;
}
```

---

### **Abstract Classes**

An abstract class is a class with at least one pure virtual function. It cannot be instantiated.

**Example:**

```cpp
#include <iostream>
using namespace std;

class Abstract {
public:
    virtual void display() = 0; // Pure virtual function
};

class Derived : public Abstract {
public:
    void display() {
        cout << "Abstract class function implemented!" << endl;
    }
};

int main() {
    Derived obj;
    obj.display();
    return 0;
}
```

---

### **Polymorphism**

#### **1. Compile-Time Polymorphism**

Achieved through function and operator overloading.  
(Refer to Unit 4 examples for overloading.)

#### **2. Runtime Polymorphism**

Achieved using virtual functions.

**Example:**

```cpp
#include <iostream>
using namespace std;

class Base {
public:
    virtual void show() {
        cout << "Base class function" << endl;
    }
};

class Derived : public Base {
public:
    void show() override {
        cout << "Derived class function" << endl;
    }
};

int main() {
    Base *ptr;
    Derived obj;
    ptr = &obj;
    ptr->show(); // Calls Derived's function
    return 0;
}
```

---

### **“this” Pointer**

A pointer to the calling object.

**Example:**

```cpp
#include <iostream>
using namespace std;

class Example {
public:
    void display() {
        cout << "Address of object: " << this << endl;
    }
};

int main() {
    Example obj;
    obj.display();
    return 0;
}
```

---

### **Pointer to Derived Classes**

A base class pointer can point to a derived class object.

**Example:**

```cpp
#include <iostream>
using namespace std;

class Base {
public:
    virtual void show() {
        cout << "Base class" << endl;
    }
};

class Derived : public Base {
public:
    void show() override {
        cout << "Derived class" << endl;
    }
};

int main() {
    Base *ptr = new Derived();
    ptr->show(); // Calls Derived's function
    delete ptr;
    return 0;
}
```

---

## **Unit 6: Exception Handling**

### **Concept of Exception Handling**

Exception handling allows managing runtime errors using `try`, `catch`, and `throw` blocks.

---

### **Syntax**

```cpp
try {
    // Code that may throw an exception
} catch (type exception) {
    // Handle exception
} catch (...) {
    // Handle all exceptions
}
```

---

### **Examples**

#### **1. Handling Divide by Zero**

```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cout << "Enter two numbers: ";
    cin >> a >> b;

    try {
        if (b == 0)
            throw "Division by zero!";
        cout << "Result: " << a / b << endl;
    } catch (const char *e) {
        cout << "Error: " << e << endl;
    }

    return 0;
}
```

---

#### **2. Catching All Exceptions**

```cpp
#include <iostream>
using namespace std;

int main() {
    try {
        throw 20;
    } catch (...) {
        cout << "An exception occurred!" << endl;
    }

    return 0;
}
```

---

#### **3. Custom Exception Handling**

```cpp
#include <iostream>
#include <string>
using namespace std;

class MyException : public exception {
    string message;

public:
    MyException(string msg) : message(msg) {}
    const char *what() const throw() {
        return message.c_str();
    }
};

int main() {
    try {
        throw MyException("Custom Exception");
    } catch (MyException &e) {
        cout << "Caught: " << e.what() << endl;
    }

    return 0;
}
```

---

