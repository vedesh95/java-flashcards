# Java Data Types Flashcard

---

## 🌟 Summary / Overview

Java provides a set of built-in data types known as **primitive types**, along with reference types (objects). Data types define the size, behavior, and allowed operations for variables.

### Primitive Data Types
| Type    | Size (bits) | Range / Notes                        |
|---------|-------------|---------------------------------------|
| byte    | 8           | -128 to 127                          |
| short   | 16          | -32,768 to 32,767                    |
| int     | 32          | -2^31 to 2^31-1                      |
| long    | 64          | -2^63 to 2^63-1                      |
| float   | 32          | ~6-7 decimal digits precision         |
| double  | 64          | ~15 decimal digits precision         |
| char    | 16          | Unicode characters (0 to 65,535)     |
| boolean | JVM dependent | true / false                        |

### Reference Types
Reference types store references to objects (instances of classes, arrays, etc.) rather than actual data.

Other notes:
- Default values for primitives: 0, 0.0, '\u0000', false
- Default value for references: null
- Java is **strongly typed**; variables must be declared with a type.

---

## 🌟 Quiz Questions

1️⃣ What are Java's primitive data types? List them.

2️⃣ What is the size and range of `int` in Java?

3️⃣ What is the default value of a `boolean` field in Java?

4️⃣ How many bits does a `char` occupy in Java, and what does it represent?

5️⃣ What is the difference between primitive types and reference types?

6️⃣ Why is Java called a strongly typed language?

7️⃣ What is the default value of an object reference?

---

## 🌟 Answers

1️⃣ Java's primitive data types: byte, short, int, long, float, double, char, boolean.

2️⃣ `int` is 32 bits, range: -2^31 to 2^31-1.

3️⃣ `boolean` default: false.

4️⃣ `char` is 16 bits, represents Unicode characters (0 to 65,535).

5️⃣ Primitive types store actual values; reference types store memory addresses of objects.

6️⃣ Java requires variables to be declared with a type and enforces type checking at compile time.

7️⃣ Default value of an object reference is `null`.

