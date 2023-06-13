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


## Simple Java:
Data Types:
Data types specify the different sizes and values that can be stored in the variable. There are two types of data types in Java:

**Primitive data types: **
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
**Non-primitive/ Reference/ Object Data Types:** The non-primitive data types include Classes, Interfaces, and Arrays.

**There are three kinds of variables in Java**
1. **Local variables -** declared in methods, constructors, or blocks.
3. **Instance variables -** Ideclared in a class, but outside a method, constructor or any block.
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



























