---
title: Learn CPP
date: 2024-12-02
draft: false
tags:
  - cpp
  - programming
---

## 🌟 **Learning C++ from Beginner to Advanced**

Welcome to this journey of mastering **C++**! 🚀 Whether you're just starting or looking to level up, this guide has you covered. Let's dive into the world of **C++ programming**, step by step.
<!--more-->

---

## 🟢 **1. Getting Started: Hello, World!**

C++ is a versatile and powerful language used for developing games, software systems, and even embedded systems. Here's your first program:

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, World!" << endl;
    return 0;
}
```

💡 **Explanation**:

- `#include <iostream>`: Adds input/output functionalities.
- `cout`: Used to print text.
- `endl`: Moves to the next line.

---

## 🔵 **2. Basics: Variables and Data Types**

C++ offers various **data types** to store values. Here's an example:

```cpp
#include <iostream>
using namespace std;

int main() {
    int age = 20;          // Integer
    float height = 5.9;    // Float
    char grade = 'A';      // Character
    string name = "Alex";  // String
    bool isStudent = true; // Boolean

    cout << "Name: " << name << endl;
    cout << "Age: " << age << endl;
    cout << "Height: " << height << endl;
    cout << "Grade: " << grade << endl;
    cout << "Is Student: " << isStudent << endl;

    return 0;
}
```

🎨 **Pro Tip**: Use different **data types** to optimize memory usage!

---

## 🟡 **3. Control Structures: If-Else and Loops**

### **If-Else Example**

```cpp
#include <iostream>
using namespace std;

int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;

    if (num % 2 == 0) {
        cout << num << " is even." << endl;
    } else {
        cout << num << " is odd." << endl;
    }

    return 0;
}
```

### **For Loop Example**

```cpp
#include <iostream>
using namespace std;

int main() {
    for (int i = 1; i <= 5; i++) {
        cout << "Count: " << i << endl;
    }

    return 0;
}
```

---

## 🟣 **4. Functions and Pointers**

Functions help break down your code into reusable blocks.

```cpp
#include <iostream>
using namespace std;

int add(int a, int b) {
    return a + b;
}

int main() {
    int x = 5, y = 10;
    cout << "Sum: " << add(x, y) << endl;

    return 0;
}
```

**Pointers** allow you to work with memory directly:

```cpp
#include <iostream>
using namespace std;

int main() {
    int var = 42;
    int* ptr = &var;  // Pointer to var

    cout << "Value: " << var << endl;
    cout << "Address: " << ptr << endl;
    cout << "Value via Pointer: " << *ptr << endl;

    return 0;
}
```

---

## 🔴 **5. Object-Oriented Programming (OOP)**

C++ supports **classes and objects**, enabling OOP principles.

```cpp
#include <iostream>
using namespace std;

class Car {
public:
    string brand;
    int speed;

    void display() {
        cout << "Brand: " << brand << ", Speed: " << speed << " km/h" << endl;
    }
};

int main() {
    Car car1;
    car1.brand = "Tesla";
    car1.speed = 200;

    car1.display();

    return 0;
}
```

---

## 🟠 **6. Advanced Topics: STL and File Handling**

### **Standard Template Library (STL)**

The STL provides pre-built classes and functions like `vector` and `map`:

```cpp
#include <iostream>
#include <vector>
using namespace std;

int main() {
    vector<int> numbers = {1, 2, 3, 4, 5};

    for (int num : numbers) {
        cout << num << " ";
    }
    cout << endl;

    return 0;
}
```

### **File Handling**

```cpp
#include <iostream>
#include <fstream>
using namespace std;

int main() {
    ofstream file("example.txt");
    file << "Learning C++ is fun!" << endl;
    file.close();

    ifstream readFile("example.txt");
    string line;
    while (getline(readFile, line)) {
        cout << line << endl;
    }
    readFile.close();

    return 0;
}
```

---

## 🎉 **Final Words**

You've taken the first steps into **C++ programming**! From basic syntax to advanced OOP, there's so much more to explore. Keep practicing, and soon you'll be creating **powerful applications**.

🔗 _Happy Coding!_ 😊
