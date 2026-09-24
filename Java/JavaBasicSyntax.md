# Java Basic Syntax

- [Java Syntax](#java-syntax)
- [Data Types](#data-types)
- [Variable Declaration](#variable-declaration)

---
# Java Syntax
Java class definition
```java
public class Main{}
```
> public - Java access modifier
>
> class - Java keyword 
>
> Main­ - Identifier, a user defined name or label ( Eg. MyClass, Hellokitty, MaaMaaaa ). Should always start with capital letter.

This function definition will be the entry point of the program and will be placed inside the "_Main class_".
```java
public static void main( String[] args ){}
``` 
> public - Java access modifier
>
> static - Non-access modifier keyword for methods and attributes.
>
> void - Return data type
>
> main - A required method identifier for program entry point.

When put together it will look like... ```Main class{ main method }```
```java
public class Main{ public static void main( String[] args ){} }
```
- Note that the ```Main``` class and ```main``` method inside it are different identifiers
- The ```Main``` inside ```public class Main``` is a custom identifier, you can change it but the source code's file name should also be saved under this class name.
> Example : 
>
> public class Main{} -> saved to _Main.java_
>
> public class HelloKitty{} -> saved to _HelloKitty.java_
- While the ```main``` inside the ```public static void main( String[] args )``` is a fixed identifier.
---
## Writing code
The source code can be written on a single line or multiline with indentations.
- Single line
```java
public class Main{ public static void main( String[] args ){} }
```
- Multiline with inconsistent indentations
```java
public class Main{ 
         public static void main( String[] args ){
// Comment - start of program
  } 
    }
```
- We can write codes like this and it will run perfectly fine since Java compiler isn't strict and sensitive on white spaces.

But for the sake of readability, we use proper and consistent indentation.
> We use tabs or spaces to indent
```java
public class Main{
    public static void main( String[] args ){
        // Comment - start of program
    } 
}
```

---
## Data Types

### Primitive Data types
| Type | Value |
|-|-|
| char | Single characters enclosed with singe quotes( e.g., 'a' 'b' '!' '$') |
| byte | -128 to 127 |
| short | -32,768 to 32,767 |
| int| -2,147,483,648 to 2,147,483,647 |
| long | ±9.22e18 |
| float | 3.141592 |
| double | 3.1415926535897932 |

### Reference Data types
| Type | Description |
|-|-|
| String | Sequence of characters enclosed with double quotes( e.g., "Some phrase" )
| Scanner | A Java class located in java.util package
---

# Variable Declaration
- Syntax = datatype identifier
```java
int number;
```
> int - Data type
>
> number - User defined identifier
>
> semicolon( ; ) - Used as a line ender

- We can declare multiple variables with different types.
```java
int number;
boolean areUsure;
char character;
```
> This can be done multilne or on a single line
```java
int number; boolean areUsure; char character;
```
You can also make this multi-line declaration of variables with same type on a single line.
```java
int numOne;
int numTwo;
int numThree;
```
or
```java
int numOne, numTwo, numThree;
```
> The data type is omitted and variables are separated with comma.

Actual source code
```java
public class Main{ 
    public static void main( String[] args ){
        // We can declare multiple variables with different types.
        int number;
        boolean areUsure;
        char character;

        // You can also write declaration of variables with same data type on a single line.
        int numOne, numTwo, numThree;
        // The data type is omitted and variables are separated with comma.
    } 
}
```
