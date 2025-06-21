# Java Methods and Varargs Flashcard

---

## 🌟 Summary / Overview

### Java Methods

- A method in Java is a block of code that performs a specific task and can be invoked when needed.
- Methods promote code reuse, modularity, and clarity.
- Syntax:

```java
modifier returnType methodName(parameterList) { 
    // body
}
```

- Parameters can be primitive types, reference types, or varargs.

### Varargs (Variable Arguments)

- Varargs allow a method to accept **zero or more arguments** of a specified type.
- Declared with an ellipsis `...`:

```java
public void printNumbers(int... numbers) {
    for (int num : numbers) {
        System.out.println(num);
    }
}
```

- Behind the scenes, Java treats varargs as an array.
- Rules:
  - Only **one varargs parameter** is allowed per method.
  - Varargs must be the **last parameter** in the method signature.

---

## 🌟 Quiz Questions

1️⃣ What is a method in Java?

2️⃣ What are the benefits of using methods?

3️⃣ What are varargs in Java?

4️⃣ How do you declare a method with varargs?

5️⃣ How are varargs treated internally?

6️⃣ Can you have more than one varargs parameter in a method?

7️⃣ Where must the varargs parameter appear in the method signature?

---

## 🌟 Answers

1️⃣ A method is a block of code designed to perform a particular task and can be called/invoked as needed.

2️⃣ Methods help with code reuse, readability, maintainability, and modular design.

3️⃣ Varargs (variable arguments) allow a method to accept an arbitrary number of arguments of a specified type.

4️⃣ By using an ellipsis (`...`), e.g., `void printNumbers(int... numbers)`.

5️⃣ Internally, varargs are treated as arrays.

6️⃣ No, only one varargs parameter is allowed per method.

7️⃣ The varargs parameter must be the last parameter in the method declaration.

