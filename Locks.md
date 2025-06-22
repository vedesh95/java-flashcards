# 📝 Java Concurrency: Types of Locks + Key Methods

## 🔑 Types of Locks

| **Lock Type**                | **Description**                                    | **Key Features** |
|------------------------------|----------------------------------------------------|-----------------|
| **Intrinsic Lock (Monitor Lock)** | Built-in lock via `synchronized` keyword            | Implicit lock/unlock, reentrant, no fairness, no interruptible acquisition, supports `wait/notify` |
| **ReentrantLock**             | Explicit lock (`java.util.concurrent.locks.ReentrantLock`) | Manual lock/unlock, reentrant, optional fairness, supports `lockInterruptibly`, `tryLock`, `Condition` |
| **ReentrantReadWriteLock**    | Separate locks for reading and writing            | Multiple readers allowed if no writer holds lock; improves read-heavy performance |
| **StampedLock (Java 8)**      | Advanced lock with optimistic reading support     | Provides optimistic read, read, and write locks; lower overhead for read-dominant scenarios |

---

## 🔑 `lockInterruptibly()`
- Acquires lock, but allows the thread to be interrupted while waiting.
- Throws `InterruptedException` if interrupted during lock wait.
- Useful for responsive shutdowns or deadlock recovery.

```java
lock.lockInterruptibly();
try {
  // critical section
} finally {
  lock.unlock();
}
