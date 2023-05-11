# OOP (Object Oriented Programming)

## Interfaces and abstract classes
1. An interface cannot implement anything. Also a class cannot extend any interface.
    ```java
    public interface Interface1 implements Class1{
        // ❌ No implements clause allowed for interface
    }
    ```

    ```java
    public class Class1 extends Interface1 {
        // ❌ No interface expected here
    }
    ```

1. An interface can extend multiple interfaces.
    ```java
    public interface Interface3 extends Interface1, Interface2{
        // An interface can extend multiple interfaces
    }
    ```
1. A class can implement multiple interfaces. However, a class can only extend a single class. Because *Java does not support multiple inheritance*.
    ```java
    public abstract class Class1 implements Interface1, Interface2 {
        // A class can implement multiple interfaces
    }
    ```

    ```java
    public abstract class Class1 extends Class2, Class3 {
        // ❌ Class cannot extend multiple classes
    }
    ```
1. An abstract class can implement multiple interfaces, but cannot extend any interface.
    ```java
    public abstract class Class1 implements Interface1, Interface2 {
        // ⚠️ abstract class can implement multiple interfaces
    }
    ```

    ```java
    public abstract class Class1 extends Interface1 {
        // ❌ No interface expected here
    }
    ```

## Difference between interface and abstract class

| Feature | Interface | Abstract Class |
|---|---|---|
| Can have abstract and non-abstract methods | Yes | Yes |
| Can implement multiple interfaces | Yes | Yes |
| Can have variables | No | Yes |
| Can extend another class | No | Yes |
