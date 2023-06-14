# java-cheat-sheet
# Features of Java:
1. Simple
2. Object-Oriented
3. Portable
4. Platform independent
5. Secured
6. Robust
7. Architecture neutral
8. Interpreted
9. High Performance
10. Multithreaded
11. Distributed
12. Dynamic
Details: https://www.javatpoint.com/features-of-java


# Simple Java:
## Data Types:
Data types specify the different sizes and values that can be stored in the variable. There are two types of data types in Java:

**Primitive data types:**
```java
byte myNum = 5;
short myNum = 10;
int myNum = 150;
long myNum = 22000
float myFloatNum = 5.99f;
char myLetter = 'D';
boolean myBool = true;
String myText = "Hello";
final int myNum = 15; // unchangeable and read-only
```
**Non-primitive/ Reference/ Object Data Types:** Classes, Interfaces, and Arrays.

**There are three kinds of variables in Java**
1. **Local variables -** declared inside methods, constructors, or blocks.
3. **Instance / Non-Instance variables -** Ideclared in a class, but outside a method, constructor or any block.
4. **Class/Static variables -** Class variables also known as static variables are declared with the static keyword in a class, but outside a method, constructor or a block.
```java
public class Hello {
    public static int phone = 999; // static variable can use without creating object/instance
    public int code = 111; // Not-Static variable needs creating object/instance to use

    public static void main(String[] args) {
        int age = 30; // Local Variable only use inside this block
        System.out.println(age);
        System.out.println(phone);

        Hello myInfo = new Hello();
        System.out.println(myInfo.code); // Not Static

    }
}
```
## Type Casting:
Convert one data type to another type.

**Implicit casting/ Widening Casting (automatically) -** converting a smaller type to a larger type size
```java 
byte -> short -> char -> int -> long -> float -> double 
```

**Explicit type casting/ Narrowing Casting (manually) -** converting a larger type to a smaller size type
```java 
double -> float -> long -> int -> char -> short -> byte 
```
```java
public class Hello {
    public static void main(String[] args) {
        int age = 30;
        double age2 = (double) age;
        System.out.println(age2); // 30.0 auto converted from int to double (smaller to larger)

        double code = 20.99;
        int code2 = (int) code;
        System.out.println(code2); // 20 manually converted from double to int (larger to smaller)
    }
}
```
### Java wrapper class:
`intValue(), byteValue(), shortValue(), longValue(), floatValue(), doubleValue(), charValue(), booleanValue().
toString()`
```java
public class Hello {
    public static void main(String[] args) {
        Integer myInt = 5;
        Double myDouble = 7.99;
        String myString = myInt.toString(); // convert other type to string

        System.out.println(myInt.doubleValue()); // 5.0
        System.out.println(myDouble.intValue()); // 7

    }
}
```

## User Input:

```java
// Using BufferReader
BufferedReader reader = new BufferedReader(new InputStreamReader(System.in));
String name = reader.readLine();

// Using Scanner
Scanner in = new Scanner(System.in);
String s = in.nextLine();
int a = in.nextInt();

// Using Console
String name = System.console().readLine();
```

## Conditional Statement:
**Java If ... Else:**
```java 
public class Hello {
    public static void main(String[] args) {
        int j = 10;
        if (j == 10) {
            System.out.println("I get printed");
        } else if (j > 10) {
            System.out.println("I don't");
        } else {
            System.out.println("I also don't");
        }
    }
}
```
**Short Hand If...Else (Ternary Operator):**
```java 
        String result = (x > 18) ? "Good day." : "Good evening.";
        System.out.println(result);
```
**Switch Statement:**
```java
public class Hello {
    public static void main(String[] args) {
        int month = 2;
        switch (month) {
            case 1:
                System.out.println("January");
                break;
            case 2:
                System.out.println("February"); // February
                break;
            default:
                System.out.println("Some other month");
                break;
        }
    }
}
```
## Java Loops:
**For Loop:**
```java
public class Hello {
    public static void main(String[] args) {
        for (int i = 1; i < 10; i++) {
            System.out.println(i); // 0123456789
        }
        
        // Break Statement
         for (int i = 0; i < 10; i++) {
            if (i == 2) {
                break; // stop all from i = 2
            }
            System.out.println(i); // 0 1
        }

        // Continue Statement
        for (int i = 0; i < 5; i++) {
            if (i == 2) {
                continue; // skip when i = 2
            }
            System.out.println(i); // 0 1 3 4
        }
    }
}
```
**While Loop:**
```java
public class Hello {
    public static void main(String[] args) {
        int i = 0;
        while (i < 10) {
            System.out.print(i); // 0 1 2 3 4 5 6 7 8 9
            i++;
        }

    }
}
```
























