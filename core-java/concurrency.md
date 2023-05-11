# Concurrency

## Quick Notes
1. The two ways of implementing thread in java are extending the `Thread` class and implementing the `Runnable` interface.
1. A race condition is a condition in which two or more threads compete together to get certain shared resources. There are two types of race conditions:
    - Read-modify-write
    - Check-then-act
1. A deadlock in Java is a situation where two or more threads are blocked and waiting for each other to release a resource, resulting in a standstill where none of the threads can continue execution.
1. Volatile variables are read directly from memory rather`volatile` keyword cannot be used with classes and methods, can be used only with variables.
1. A thread cannot be restarted. If we try to start a thread again, it throws `IllegalThreadStateException`.
1. The `synchronized` keyword can be used to perform synchronization on any specific resource of the method. Only one thread at a time can execute on a particular resource, and all other threads which attempt to enter the synchronized block are blocked.
1. Synchronized block is more preferred way because it doesn't lock the Object, synchronized methods lock the Object and if there are multiple synchronization blocks in the class, even though they are not related, it will stop them from execution and put them in wait state to get the lock on Object.