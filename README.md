# Java
This repository contains basic Java programs and examples intended for beginners transitioning from C++ or starting with Java.

- Every java program should have atleast one **public class** and name of the class should match with file name.
- Every application will have a main method and syntax for that is below
```java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello World!");
  }
}
```
- Compilation : Compiler used is javac and this compiler coverts java code into byte code.
- Execution : Bytecode is executed by converting into machine code (JVM)
### Datatypes & Variables
- Variable types should be known in compile time.
- Data types in Java are of different sizes and values that can be stored in a variable.
- There are two types of datatypes
  1. Primitive data types like boolean, char, int, byte, float, double, long
  2. Non-primitive data types like String, Class, Array etc.
```java
public class Geeks {
    public static void main(String[] args) {
        double pi = 3.141592653589793;
        System.out.println("Value of Pi: " + pi);   
    }
}
```
- type followed by name (like int num;)
- we can't declare static variable locally
```java
class Geeks {
    // Declared static variable which is crrect
    public static String name = "Rishitha Patel";
  
    public static void main(String[] args)
    {
        static int num = 0;
        //the above line throws an error
    }
}
```
### Common mistakes we usually do
- Accessing a local variable without initializing it leads to a compile-time error(no feauture like that in cpp).
- Use `==` for comparing **primitive values**, and use `.equals()` for comparing **object contents** like Strings.

### Operators
- Most of operators are same as cpp (== is an exception).

### Decision making & loops
- if-else , switch statements .. same as cpp.


### Array and HashMap declarations
```java
import java.util.ArrayList;
import java.util.HashMap;

public class array {
    public static void main(String[] args){
        ArrayList<Integer> arr = new ArrayList<>();
        arr.add(20);
        arr.add(30);
        for(int i=0;i<arr.size();i++){
            System.out.print(arr.get(i)+" ");
        }
        //using hash map
        HashMap<String,Integer> mp = new HashMap<>();
        mp.put("rishita",1);
        mp.put("sagar",2);
        //print the things in map
        for(String name : mp.keySet()){
            System.out.print(name+" ");
        }
    }
}

```
