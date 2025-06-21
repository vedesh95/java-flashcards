Java JDK, JRE, JVM Flashcard

🌟 Summary / Overview

Java development and runtime environments consist of three major components that work together:

1️⃣ Java Virtual Machine (JVM)

The JVM is the engine that runs Java bytecode.

It provides platform independence by interpreting or compiling (via JIT) bytecode to native machine code.

Handles memory management (heap, stack), garbage collection, and security.

2️⃣ Java Runtime Environment (JRE)

The JRE is what you need to run Java programs.

Contains the JVM + standard class libraries + supporting files.

Does not include development tools like javac.

3️⃣ Java Development Kit (JDK)

The JDK is for developing Java applications.

Contains JRE + development tools (e.g., javac, javadoc, debugger).

JIT Compiler

The Just-In-Time compiler is part of the JVM (inside JRE).

Converts frequently used bytecode into native machine code at runtime for better performance.

Diagram

JDK = JRE + development tools
JRE = JVM + standard libraries
JVM = Execution engine (includes JIT, garbage collector, etc.)

🌟 Quiz Questions

1️⃣ What is the role of the JVM?

2️⃣ What does the JRE include?

3️⃣ How is the JDK different from the JRE?

4️⃣ Where does the JIT compiler fit in the Java architecture?

5️⃣ Can you run a Java program with just the JDK?

6️⃣ What does the JVM provide to ensure platform independence?

🌟 Answers

1️⃣ The JVM runs Java bytecode, handles memory, and manages runtime execution.

2️⃣ The JRE includes the JVM, standard class libraries, and supporting files needed to run Java apps.

3️⃣ The JDK contains the JRE plus development tools like compilers and debuggers.

4️⃣ The JIT compiler is part of the JVM's execution engine, translating bytecode to native code at runtime.

5️⃣ Yes — the JDK includes the JRE, so you can both compile and run Java programs.

6️⃣ The JVM interprets or compiles bytecode into native instructions, allowing the same bytecode to run on any platform with a JVM.

