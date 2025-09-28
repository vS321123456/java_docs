# 📘 Object-Oriented Programming (OOP)

## 📝 Definition

Object-Oriented Programming (OOP) is a programming paradigm where software is structured around **objects** rather than functions or logic.

An **object** represents a real-world entity (like a Car, BankAccount, or Student).

Objects have **state** (fields/attributes) and **behavior** (methods/functions).

Java is a pure OOP language (with some exceptions like primitive types).

The four main pillars of OOP are:

- **Encapsulation** – Binding data and methods together.
- **Abstraction** – Hiding implementation details and exposing only necessary functionality.
- **Inheritance** – Reusing code by deriving new classes from existing ones.
- **Polymorphism** – One name, many forms (method overloading/overriding).

---

## 🎯 Example / Illustration

Think of a **Car** 🚗:

- **State** → color, brand, speed, fuel level.
- **Behavior** → `start()`, `accelerate()`, `brake()`.

Instead of writing separate functions and global variables, OOP bundles them into a single Car object.

---

## 💻 Sample Code (Java)

```java
// A simple OOP example in Java
class Car {
    // State (fields)
    String brand;
    String color;
    int speed;

    // Constructor
    Car(String brand, String color) {
        this.brand = brand;
        this.color = color;
        this.speed = 0; // initially stopped
    }

    // Behavior (methods)
    void start() {
        System.out.println(brand + " is starting...");
    }

    void accelerate(int increase) {
        speed += increase;
        System.out.println(brand + " is now running at " + speed + " km/h");
    }

    void brake() {
        speed = 0;
        System.out.println(brand + " has stopped.");
    }
}

// Main class
public class OOPExample {
    public static void main(String[] args) {
        Car car1 = new Car("Tesla", "Red");
        car1.start();
        car1.accelerate(60);
        car1.brake();
    }
}


# 🔑 Key Points

- **OOP makes code modular, reusable, and easier to maintain.
- **Encourages modeling programs around real-world objects.
- **Java heavily relies on OOP principles for frameworks like Spring, Hibernate, etc.
- **Four pillars (Encapsulation, Abstraction, Inheritance, Polymorphism) form its backbone.
