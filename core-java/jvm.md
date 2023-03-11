# Quick Notes
1. The JVM uses a Just-In-Time (JIT) compiler to convert Java bytecode into machine code, which improves performance by optimizing frequently executed code paths.
1. The JVM uses a generational garbage collection strategy, where objects are allocated in a young generation and then moved to an old generation if they survive multiple garbage collection cycles.
1. All other threads in the application have to be stopped to allow the garbage collector thread to effectively do its work.
1. This problem can be greatly reduced or even eliminated through skillful optimization and garbage collector tuning and using different GC algorithms.
1. The JVM provides a number of tools for monitoring and profiling Java applications, including jconsole, jvisualvm, and jmap.
1. The JVM provides support for dynamic class loading through the use of the Class.forName() method, which loads a class at runtime.

# Top Questions

1. How does the JVM handle memory management, and what are the different memory areas allocated by the JVM?
1. How does the JVM handle garbage collection, and what are the different garbage collection algorithms available in the JVM?
1. What is JIT compiler, and how does it improve the performance of Java programs running on the JVM?
1. What is class loading, and what are the different types of class loaders available in the JVM?
1. What is bytecode, and how does the JVM interpret and execute bytecode instructions?
1. How does the JVM handle exceptions, and what is the role of the exception table in the class file format?
1. What is the difference between JVM, JRE, and JDK, and how do they relate to each other?
1. How does the JVM handle multi-threading, and what are the different synchronization mechanisms available in Java?
1. How does the JVM handle optimization, and what are the different optimization techniques used by the JVM?
1. What are some common JVM performance tuning techniques, and how do they impact the overall performance of Java programs?

# Java Class Loader
![image](https://user-images.githubusercontent.com/2513990/202668847-f895c4db-f2b4-405e-92fa-ccbc76cd4546.png)

Image courtesy: DZone


# Different Garbage Collector Algorithms in Java

Java uses various garbage collector algorithms to manage memory allocation and deallocation of objects. The most commonly used garbage collector algorithms in Java are:

1. Serial Collector: The simplest garbage collector algorithm that uses a single thread for garbage collection.
2. Parallel Collector: This garbage collector algorithm uses multiple threads to perform garbage collection, which can improve the overall performance of the application.
3. CMS (Concurrent Mark Sweep) Collector: This garbage collector algorithm performs garbage collection concurrently with the application threads, minimizing the pauses caused by garbage collection.
4. G1 (Garbage-First) Collector: This garbage collector algorithm uses a combination of parallel and concurrent garbage collection techniques to improve performance and reduce garbage collection pauses.
5. Z Garbage Collector (ZGC): This garbage collector algorithm is designed to provide low-latency garbage collection for large heaps, making it ideal for high-performance applications.

Each garbage collector algorithm has its advantages and disadvantages, and the selection of the appropriate algorithm depends on the specific requirements of the application. Java allows developers to configure the garbage collector algorithm based on the application's needs, through the use of command-line arguments or configuration files.

