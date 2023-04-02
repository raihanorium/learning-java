# Learning Java Development Ecosystem
## Covering the following topics

- Core Java 
    - [JVM](/core-java/jvm.md)
    - [Collections](/core-java/collections.md)
    - Generics
        1. One advantage of using generics is avoiding casts and provide type safety.
        1. Without generics, we have to copy and paste the same code but for different types.
        1. Type erasure means that generic type information is not available to the JVM at runtime, only compile time.
        1. When we use bounded parameters, we are restricting the types that can be used as generic type arguments.
            ```java
            public abstract class Cage<T extends Animal> {
                abstract void addAnimal(T animal)
            }
            ```
        1. Declaring multiple bounds for generic types is possible.
            ```java
                public abstract class Cage<T extends Animal & Comparable>
            ```
            If the type were a subclass of animal but did not implement comparable, then the code would not compile.
            
    - Concurrency
        1. The two ways of implementing thread in java are extending the `Thread` class and implementing the `Runnable` interface.
        1. A race condition is a condition in which two or more threads compete together to get certain shared resources. There are two types of race conditions:
            - Read-modify-write
            - Check-then-act
        1. A deadlock in Java is a situation where two or more threads are blocked and waiting for each other to release a resource, resulting in a standstill where none of the threads can continue execution.
        1. Volatile variables are read directly from memory rather`volatile` keyword cannot be used with classes and methods, can be used only with variables.
        1. A thread cannot be restarted. If we try to start a thread again, it throws `IllegalThreadStateException`.
        1. The `synchronized` keyword can be used to perform synchronization on any specific resource of the method. Only one thread at a time can execute on a particular resource, and all other threads which attempt to enter the synchronized block are blocked.
        1. Synchronized block is more preferred way because it doesn't lock the Object, synchronized methods lock the Object and if there are multiple synchronization blocks in the class, even though they are not related, it will stop them from execution and put them in wait state to get the lock on Object.

    - IO
    - Stream API
    - Regular Expressions
    - Exception Handling
    - Servlet API
    - JPA
    - OOP
    - [SOLID Principles](/core-java/solid.md)
    - Design Patterns
- Spring    
    - IOC and DI
    - Spring Boot
    - MVC
    - Security
    - OAuth
    - Batch
    - Caching
    - Hibernate
    - Flyway
- Microservice
    - DDD
    - CQRS
    - SAGA
    - Transaction
- Database    
    - ORM
    - ACID
    - Transactions
    - Database concurrency
    - N+1 Problem
    - Replication
    - Sharding
    - CAP Theorem
    - Isolation levels
- System Design
- Networking  
    - Layers
    - HTTP
    - SSL
    - DNS
    - Domains
- Unit Testing    
- Version Control 
- SAML    
- Messaging
- Logging 
- Elasticsearch   
- Agile
- Application Server
    - Tomcat
    - Nginx
- Docker
- Kubernetes
- AWS
