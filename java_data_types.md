# Java Data Types Flashcard

---

## 🌟 Summary / Overview

Java provides two broad categories of data types: **primitive types** and **reference types**.

### Primitive Data Types

| Type    | Size (bits)   | Range / Notes                    |
| ------- | ------------- | -------------------------------- |
| byte    | 8             | -128 to 127                      |
| short   | 16            | -32,768 to 32,767                |
| int     | 32            | -2^31 to 2^31-1                  |
| long    | 64            | -2^63 to 2^63-1                  |
| float   | 32            | \~6-7 decimal digits precision   |
| double  | 64            | \~15 decimal digits precision    |
| char    | 16            | Unicode characters (0 to 65,535) |
| boolean | JVM dependent | true / false                     |

![image](https://github.com/user-attachments/assets/2b0f0ebf-cad5-49f7-89ad-724f03524699)

### Reference Data Types (Detailed)

Reference types store **memory addresses (references)** to actual objects, not the object’s data directly. The types that fall under reference types include:

- **Classes**: Any instance of a class (e.g., `String`, `Scanner`, `ArrayList`).
- **Interfaces**: Variables declared as an interface type can reference objects of classes implementing that interface.
- **Arrays**: Arrays of primitive or reference types are themselves objects.
- **Enums**: Special reference types that define a set of constants.

#### Key points about reference types:

- The value stored in the variable is the address pointing to the object in memory.
- Access to the actual data is done through this reference.
- When you assign one reference variable to another, both point to the same object.
- The default value for reference types is `null`.
- `null` means the reference does not point to any object.

### Autoboxing and Unboxing

- **Autoboxing**: Automatic conversion of a primitive type to its corresponding wrapper class (e.g., `int` → `Integer`).
- **Unboxing**: Automatic conversion of a wrapper class object back to its corresponding primitive type.
- These conversions happen implicitly, for example:

```java
Integer obj = 5;  // autoboxing of int 5 to Integer
int num = obj;    // unboxing Integer to int
```

### String Pool

- The **String pool** (or intern pool) is a special memory region where Java stores string literals.
- If two string literals have the same content, they share the same object in the pool.
- Example:

```java
String a = "hello";
String b = "hello";
System.out.println(a == b); // true, same pool object
```

- Using `new String("hello")` creates a new object outside the pool.

---

## 🌟 Quiz Questions

1️⃣ What are Java's primitive data types? List them.

2️⃣ What types fall under reference data types?

3️⃣ What does a reference variable store in Java?

4️⃣ What is the default value of a reference type?

5️⃣ How are arrays treated in Java in terms of data type?

6️⃣ What happens when two reference variables point to the same object?

7️⃣ What is `null` in the context of reference types?

8️⃣ What is autoboxing and unboxing in Java?

9️⃣ What is the String pool and how does it work?

10️⃣ How does using `new String()` differ from using string literals?

---

## 🌟 Answers

1️⃣ Java's primitive data types: byte, short, int, long, float, double, char, boolean.

2️⃣ Reference data types include classes, interfaces, arrays, and enums.

3️⃣ A reference variable stores the memory address of the object it refers to.

4️⃣ The default value of a reference type is `null`.

5️⃣ Arrays are treated as objects and are reference types in Java.

6️⃣ If two reference variables point to the same object, changes made via one reference are visible through the other.

7️⃣ `null` indicates that a reference variable does not point to any object in memory.

8️⃣ Autoboxing is the automatic conversion of a primitive type to its wrapper class. Unboxing is the reverse: wrapper to primitive.

9️⃣ The String pool is a memory region that stores string literals so identical literals share the same object, saving memory.

🔟 Using `new String()` creates a new string object on the heap, not the pool, even if the content is identical to an existing string literal.

