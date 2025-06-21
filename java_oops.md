# Java OOP Concepts — Intermediate Level

---

## 🌟 Summary / Overview

Java's Object-Oriented Programming (OOP) principles form the backbone of its design, enabling modular, reusable, and maintainable code. The four key pillars of OOP in Java are:

* **Encapsulation**: Hiding internal state and requiring all interaction to be performed through an object's methods. This protects the integrity of the object's data.
* **Inheritance**: A mechanism where a new class derives properties and behavior from an existing class, supporting code reuse and hierarchical classification.
* **Polymorphism**: The ability of one interface to be used for a general class of actions. The specific action is determined by the exact nature of the situation.
* **Abstraction**: Focusing on essential qualities rather than specific characteristics. Abstraction hides complexity by exposing only relevant features through abstract classes and interfaces.

Other important related concepts include:

* **Composition**: Building classes using references to other objects (has-a relationships), often preferred over inheritance to promote flexibility.
* **Inner Classes**: Classes defined within another class, used for logically grouping classes or accessing enclosing class members.
* **Sealed Classes (Java 17)**: Classes that restrict which other classes can extend them, enhancing control over type hierarchies.
* **Covariant Return Types**: Allowing an overriding method to return a subtype of the original return type.
* **Dynamic Method Dispatch**: The process by which a call to an overridden method is resolved at runtime rather than compile time.

---

## 🌟 Quiz Mode — Questions

1️⃣ What is encapsulation in Java? Why is it important?

2️⃣ What is inheritance in Java? How is it implemented?

3️⃣ What is polymorphism? What are its types in Java?

4️⃣ What is abstraction? How is it achieved in Java?

5️⃣ What is the difference between an abstract class and an interface (Java 8+)?

6️⃣ What is method overloading vs method overriding?

7️⃣ What are the rules for method overriding in Java?

8️⃣ What is a covariant return type?

9️⃣ What is the Diamond Problem? How does Java handle it?

🔟 How does Java handle multiple inheritance with interfaces that have the same default method?

1️⃣1️⃣ What is composition? How does it compare to inheritance?

1️⃣2️⃣ What are sealed classes (Java 17)? What problem do they solve?

1️⃣3️⃣ What is an inner class? What types of inner classes exist in Java?

1️⃣4️⃣ Can constructors be inherited in Java?

1️⃣5️⃣ What is the difference between `this` and `super` in Java?

1️⃣6️⃣ How does Java achieve runtime polymorphism internally?

1️⃣7️⃣ Can a class be both abstract and final? Why or why not?

1️⃣8️⃣ What is the difference between interface default methods and abstract class methods?

---

## 🌟 Answers

1️⃣ Encapsulation is the practice of hiding an object's internal state and requiring all interaction through public methods. It ensures data integrity and provides controlled access.

2️⃣ Inheritance allows a class (subclass) to derive properties and behaviors from another class (superclass), implemented using the `extends` keyword.

3️⃣ Polymorphism means many forms. Types: compile-time (method overloading) and runtime (method overriding).

4️⃣ Abstraction hides internal implementation details and shows only relevant features. Achieved through abstract classes and interfaces.

5️⃣ Abstract classes can have constructors, state, abstract and concrete methods. Interfaces (Java 8+) can have abstract, default, and static methods, but no constructors or instance state.

6️⃣ Overloading: same method name, different parameter lists (compile-time). Overriding: subclass provides specific implementation for a superclass method (runtime).

7️⃣ Same signature, can’t reduce visibility, can return covariant types, can’t throw broader checked exceptions, can’t override final/static methods.

8️⃣ Covariant return type allows an overriding method to return a subtype of the original return type.

9️⃣ The Diamond Problem is ambiguity from multiple inheritance of classes; Java avoids this by supporting single class inheritance.

🔟 Java forces the implementing class to resolve conflicts explicitly if two interfaces provide the same default method.

1️⃣1️⃣ Composition means building classes using other objects. It’s preferred over inheritance for flexibility and looser coupling.

1️⃣2️⃣ Sealed classes restrict which classes can extend them, providing more control over inheritance hierarchies.

1️⃣3️⃣ Inner classes are classes defined inside another class. Types: static nested class, non-static inner class, local class, anonymous class.

1️⃣4️⃣ Constructors are not inherited, but a subclass can invoke a superclass constructor using `super()`.

1️⃣5️⃣ `this` refers to the current instance. `super` refers to the parent class instance.

1️⃣6️⃣ Java uses dynamic method dispatch (virtual method table) to resolve overridden methods at runtime.

1️⃣7️⃣ No. Abstract means meant to be subclassed. Final means cannot be subclassed. They are contradictory.

1️⃣8️⃣ Interface default methods provide implementation without state. Abstract class methods can use instance state and constructors.
