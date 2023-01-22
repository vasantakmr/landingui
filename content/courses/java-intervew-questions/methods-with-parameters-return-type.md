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