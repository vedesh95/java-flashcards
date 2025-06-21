# Java Memory Management & Garbage Collection Quiz Flashcard

---

## 🌟 Quiz Questions (Covers Full Theory)

1️⃣ What are the main memory areas managed by JVM, and what is stored in each?

2️⃣ What is the role of the heap in Java memory management?

3️⃣ What is stored in the stack, and how is it used during execution?

4️⃣ What is the method area (metaspace), and what does it hold?

5️⃣ What is the purpose of the PC register in JVM memory?

6️⃣ What is the native method stack used for?

7️⃣ What is a strong reference?

8️⃣ When does the garbage collector clear soft references?

9️⃣ What is a weak reference, and when is it cleared?

🔟 What is the use of a phantom reference?

1️⃣1️⃣ How is memory shared or isolated between threads in Java?

1️⃣2️⃣ What does the mark-and-sweep algorithm do?

1️⃣3️⃣ How does mark-and-compact improve over mark-and-sweep?

1️⃣4️⃣ What is copying GC, and how does it work?

1️⃣5️⃣ What is generational GC, and why is it used?

1️⃣6️⃣ When is Serial GC appropriate?

1️⃣7️⃣ What is the key advantage of Parallel GC?

1️⃣8️⃣ How does G1 GC manage heap regions?

1️⃣9️⃣ What is the key benefit of ZGC and Shenandoah?

---

## 🌟 Answers

1️⃣ Heap (objects), stack (frames, locals), method area/metaspace (class data), PC register (current instruction), native method stack (native calls).

2️⃣ The heap stores all objects and instance variables and is managed by the GC.

3️⃣ The stack stores method calls, local variables, and references to heap objects.

4️⃣ The method area/metaspace holds class metadata, static variables, and method code.

5️⃣ The PC register holds the address of the currently executing instruction for the thread.

6️⃣ The native method stack handles native (non-Java) method invocations.

7️⃣ A strong reference prevents the GC from collecting the object.

8️⃣ Soft references are cleared only when the JVM needs memory.

9️⃣ Weak references are cleared at the next GC cycle if no strong references exist.

🔟 Phantom references are used to schedule actions after finalization but before memory is reclaimed.

1️⃣1️⃣ The heap is shared between threads; stacks, PC registers, and native method stacks are thread-specific.

1️⃣2️⃣ Marks reachable objects, sweeps unmarked objects to reclaim memory.

1️⃣3️⃣ Mark-and-compact also moves live objects together, eliminating fragmentation.

1️⃣4️⃣ Copies live objects from one region (from-space) to another (to-space), leaving dead objects behind.

1️⃣5️⃣ It optimizes collection by treating short-lived and long-lived objects differently.

1️⃣6️⃣ Suitable for single-CPU machines or small heaps; simple stop-the-world behavior.

1️⃣7️⃣ Uses multiple threads to speed up collection and improve throughput.

1️⃣8️⃣ G1 GC breaks the heap into regions and prioritizes regions with most garbage for collection.

1️⃣9️⃣ They provide low-latency GC by performing most work concurrently with application threads.

