# Generics

## Quick Notes
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