---
title: Methods/Functions 
description: Breakdown of methods concept
weight: 5
lastmod: 2022-11-20T10:23:30-09:00
draft: false
youtube: tUm1AlaMcMQ
emoji: 🚀
video_length: 27:05
free: true
---
<!-- 
<quiz-modal options="Biometric:Cookies:JSON Web Token:Hashmap" answer="JSON Web Token" prize="3">
  <h6>What type of authentication mechanism does Supabase use by default?</h6>
</quiz-modal> -->

#### 1)What is method in java ?

A method in Java is a block of code that performs a specific task and can be reused multiple times in a program. Methods can be called from other parts of the program, and they can also accept parameters and return values.

It contains the executable body that can be applied to the specific object of the class.
Method includes method name, parameters or arguments and return type and a body of executable code.

Syntax : 
```java
type methodName(Argument List){
}
```

ex : public float add(int a, int b, int c) {

}
methods can have multiple arguments. Separate with commas when we have multiple arguments


#### 2) Why main() method is public, static and void in java ?

public : “public” is an access specifier which can be used outside the class. When main method is declared 
public it means it can be used outside class.

static : To call a method we require object. Sometimes it may be required to call a method without the 
help of object. Then we declare that method as static. JVM calls the main() method without creating 
object by declaring keyword static.

void : void return type is used when a method does’nt return any value . main() method does’nt return 
any value, so main() is declared as void.

Signature : public static void main(String[] args) {


#### 3) Explain about main() method in java?

Main() method is starting point of execution for all java applications.

public static void main(String[] args) {}

String args[] are array of string objects we need to pass from command line arguments.
Every Java application must have atleast one main method.


#### 4) What is difference between length and length() method in java ?

length() : In String class we have length() method which is used to return the number of characters in 
string.

Ex : 
String str = “Hello World”;
System.out.println(str.length());
Str.length() will return 11 characters including space.

length : we have length instance variable in arrays which will return the number of values or objects in 
array.

For example :
String days[]={” Sun”,”Mon”,”wed”,”thu”,”fri”,”sat”};
Will return 6 since the number of values in days array is 6.


#### 5) How do you define a method in Java?
To define a method in Java, you use the keyword public or private to specify the access level, the keyword static or not if the method is static or not, the return type, the method name, a set of parentheses that may contain parameter types and names, and a block of code inside curly braces. Example:
```java
public static int add(int a, int b) {
    return a + b;
}
```


#### 6) How do you call a method in Java?
To call a method in Java, you use the method name followed by a set of parentheses that may contain the actual values of the parameters. Example:
```java
int result = add(5, 10);
```


#### 7) What is the difference between a static method and a non-static method in Java?
A static method belongs to a class and can be called without creating an instance of the class, while a non-static method belongs to an object and can be called after creating an instance of the class.

#### 8) How do you pass parameters to a method in Java?
To pass parameters to a method in Java, you provide the actual values of the parameters in the parentheses when calling the method. The data type of the actual value should match the data type of the parameter. Example:
```java
int result = add(5, 10);
```


#### 9) How do you return a value from a method in Java?
To return a value from a method in Java, you use the keyword return followed by the value or expression that you want to return. The data type of the returned value should match the data type that is specified in the method definition. Example:
```java
public static int add(int a, int b) {
    return a + b;
}
```


#### 10) How do you overload a method in Java?
To overload a method in Java, you create multiple methods with the same name but with different parameter lists. The methods can have different numbers of parameters or different data types of parameters.

#### 11) How do you use default arguments in a method in Java?
In java, you can use default arguments by providing default values to the parameters in the method definition. If the calling method does not provide any values for these parameters, the default values will be used. Example:
```java
public static int add(int a, int b, int c = 0) {
    return a + b + c;
}
```


#### 12) How do you use variable arguments in a method in Java?
In Java, you can use variable arguments by using the ... operator followed by the parameter name in the method definition. This allows the method to accept any number of arguments of the specified data type. Example:
```java
public static int add(int... numbers) {
    int result = 0;
    for (int number : numbers) {
        result += number;
    }
    return result;
}
```


#### 13) How do you use a method that throws an exception in Java?
To use a method that throws an exception in Java, you can either use a try-catch block to handle the exception or use the throws keyword in the method signature to indicate that the method can throw a specific exception. Example:

```java
public static void myMethod() throws IOException {
    // code that can throw an IOException
}
```


#### 14) How do you use the this keyword in a method in Java?
The this keyword in Java is used to refer to the current object. It can be used to refer to the instance variables and instance methods of the current class. Example:
```java
public class MyClass {
    private int myVar;

    public void setMyVar(int myVar) {
        this.myVar = myVar;
    }
}
```


#### 15) How do you use the super keyword in a method in Java?
The super keyword in Java is used to refer to the parent class of the current class. It can be used to call the constructor of the parent class, or to access the parent class's methods or variables. Example:
```java
public class MyChildClass extends MyParentClass {
    public MyChildClass() {
        super();
    }
}
```


#### 16) How do you create a recursive method in Java?
A recursive method in Java is a method that calls itself. To create a recursive method, you use the method name within the method body to call the method again. Example:
```java
public static int factorial(int n) {
    if (n == 0) {
        return 1;
    }
    return n * factorial(n - 1);
}
```


#### 17) How do you use the final keyword to make a method unchangeable in Java?
To make a method unchangeable in Java, you can use the final keyword before the method definition. A final method can not be overridden by a subclass.

#### 18) How do you use the abstract keyword to create an abstract method in Java?
To create an abstract method in Java, you can use the abstract keyword before the method definition and do not provide an implementation. An abstract method must be overridden in a concrete class.

#### 19) How do you use the synchronized keyword to make a method thread-safe in Java?
To make a method thread-safe in Java, you can use the synchronized keyword before the method definition. This will ensure that only one thread can execute the method at a time, even if multiple threads are trying to access the method simultaneously.

#### 20) How do you use the native keyword to indicate a method is implemented in another language in Java?
To indicate a method that is implemented in another language, such as C or C++, you can use the native keyword before the method definition. This tells the Java Virtual Machine that the implementation of the method is in a different language and it will use the native libraries to execute the method.