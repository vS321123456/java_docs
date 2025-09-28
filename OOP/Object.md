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
