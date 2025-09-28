# 📘 Object in Java

## 📝 Definition

An **object** is an instance of a class.

It represents a real-world entity with **state** (attributes/fields) and **behavior** (methods).

Objects are created from **classes** (blueprints).

In memory, an object occupies space to store its data (fields) and gives access to its methods.

👉 Without objects, a class is just a definition — **objects bring it to life**.

---

## 🎯 Example / Illustration

Think of a **Class** as a blueprint of a house 🏠.

The house blueprint (class) defines structure, but it’s not a real house.

A constructed house (**object**) is a usable, real instance of the blueprint.

You can create many houses (**objects**) from the same blueprint (**class**).

---

## 💻 Sample Code (Java)

```java
// Class definition
class Dog {
    String name;   // State (field)
    int age;       // State (field)

    // Behavior (method)
    void bark() {
        System.out.println(name + " is barking!");
    }
}

public class ObjectExample {
    public static void main(String[] args) {
        // Creating objects (instances of Dog class)
        Dog dog1 = new Dog();
        dog1.name = "Tommy";
        dog1.age = 3;

        Dog dog2 = new Dog();
        dog2.name = "Bruno";
        dog2.age = 5;

        // Using objects
        dog1.bark(); // Tommy is barking!
        dog2.bark(); // Bruno is barking!
    }
}
```
---

# 📘 new Keyword in Java

## 📝 Definition

The **new** keyword in Java is used to create objects.

- It allocates memory in the heap for a new object.
- It calls the class constructor to initialize the object.
- Returns a reference (address in memory) that is stored in a variable.

👉 Without **new**, you can’t create instances of most classes (except for some special cases like reflection, cloning, or factory methods).

---

## 🎯 Example / Illustration

Think of **new** like ordering a new phone 📱 from a factory:

- You tell the factory (constructor) what model to build.
- The factory creates a fresh phone (object).
- You get the receipt (reference variable) to identify and use that phone.

---

## 💻 Sample Code (Java)

```java
class Student {
    String name;
    int age;

    // Constructor
    Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

    void displayInfo() {
        System.out.println("Name: " + name + ", Age: " + age);
    }
}

public class NewKeywordExample {
    public static void main(String[] args) {
        // Creating object using 'new'
        Student s1 = new Student("Alice", 20);
        Student s2 = new Student("Bob", 22);

        // Using objects
        s1.displayInfo(); // Name: Alice, Age: 20
        s2.displayInfo(); // Name: Bob, Age: 22
    }
}
```

