---
title: Object Oriented Principles
description: How to implement OOPS
weight: 13
lastmod: 2022-11-20T10:23:30-09:00
draft: false
vimeo: 773632911
emoji: 💅
video_length: 1:45
free: true
---


#### 1) What are static blocks and static initalizers in Java ?

Static blocks or static initializers are used to initalize static fields in java. we declare static blocks when we 
want to intialize static fields in our class. Static blocks gets executed exactly once when the class is loaded 
. Static blocks are executed even before the constructors are executed.

#### 2) How to call one constructor from the other constructor ?

With in the same class if we want to call one constructor from other we use this() method. Based on the 
number of parameters we pass appropriate this() method is called.
Restrictions for using this method :
1) this must be the first statement in the constructor
2) we cannot use two this() methods in the constructor

#### 3) What is method overriding in java ?

If we have methods with same signature (same name, same signature, same return type) in super class 
and subclass then we say
subclass method is overridden by superclass.
When to use overriding in java
If we want same method with different behaviour in superclass and subclass then we go for overriding.
When we call overridden method with subclass reference subclass method is called hiding the superclass 
method.

#### 4) What is super keyword in java ?

Variables and methods of super class can be overridden in subclass . In case of overriding , a subclass 
object call its own variables and methods. Subclass cannot access the variables and methods of 
superclass because the overridden variables or methods hides the methods and variables of super class.
But still java provides a way to access super class members even if its members are overridden. Super is 
used to access superclass variables, methods, constructors.
Super can be used in two forms :
1) First form is for calling super class constructor.
2) Second one is to call super class variables,methods.
Super if present must be the first statement.

#### 5) Difference between method overloading and method overriding in java ?

| Method Overloading  | Method Overriding  |
|---|---|
| 1) Method Overloading occurs with in the same class | 1) Method Overriding occurs between two classes superclass and subclass |
| 2) Since it involves with only one class inheritance is not involved.  | 2) Since method overriding occurs between superclass and subclass inheritance is involved. |
| 3)In overloading return type need not be the same   | 3) In overriding return type must be same.  |
| 4) Parameters must be different when we do overloading  | 4) Parameters must be same.  |
| 5) Static polymorphism can be acheived using method overloading  |  5) Dynamic polymorphism can be acheived using method overriding. |
| 6) In overloading one method can’t hide the another  |  6) In overriding subclass method hides that of the superclass method. |

#### 6) Difference between abstract class and interface ?


| Interface  | Abstract Class  |
|---|---|
| 1) Interface contains only abstract methods | 1) Abstract class can contain abstract methods, concrete methods or both |
| 2) Access Specifiers for methods in interface must be public  | 2) Except private we can have any access specifier for methods in abstract class. |
| 3) Except private variables can have any access specifiers  | 3) Variables defined must be public , static , final  |
| 4) Multiple Inheritance in java is implemented using interface  | 4)We cannot achieve multiple inheritance using abstract class.  |
| 5) To implement an interface we use implements keyword  |  5)To implement an interface we use implements keyword |


#### 7) What is method overloading in java ?

A class having two or more methods with same name but with different arguments then we say that those 
methods are overloaded. Static polymorphism is achieved in java using method overloading.

Method overloading is used when we want the methods to perform similar tasks but with different inputs 
or values. When an overloaded method is invoked java first checks the method name, and the number of 
arguments ,type of arguments; based on this compiler executes this method.

Compiler decides which method to call at compile time. By using overloading static polymorphism or static 
binding can be achieved in java.

Note : Return type is not part of method signature. we may have methods with different return types but 
return type alone is not sufficient to call a method in java.

#### 8) Difference between this() and super() in java ?

this() is used to access one constructor from another with in the same class while super() is used to 
access superclass constructor. Either this() or super() exists it must be the first statement in the 
constructor

#### 9) What is a class ?
Classes are fundamental or basic unit in Object Oriented Programming .A class is kind of blueprint or 
template for objects. Class defines variables, methods. A class tells what type of objects we are creating.

For example take Department class tells us we can create department type objects. We can create any 
number of department objects.

All programming constructs in java reside in class. When JVM starts running it first looks for the class 
when we compile. Every Java application must have atleast one class and one main method.

Class starts with class keyword. A class definition must be saved in class file that has same as class name. 
File name must end with .java extension.

{{< file "terminal" "FirstClass.java" >}}
```java 
public class FirstClass 
{
    public static void main(String[] args) 
    {
        System.out.println(“My First class”);
    }
}
```

If we see the above class when we compile JVM loads the FirstClass and generates a .class 
file(FirstClass.class). When we run the program we are running the class and then executes the main 
method.

#### 10) What is an object ?

An Object is instance of class. A class defines type of object. Each object belongs to some class.Every 
object contains state and behavior. State is determined by value of attributes and behavior is called 
method. Objects are also called as an instance.

To instantiate the class we declare with the class type.

{{< file "terminal" "FirstClass.java" >}}
```java
public class FirstClass 
{
    public static voidmain(String[] args) 
    {
        FirstClass f=new FirstClass();
        System.out.println(“My First class”);
    }
}
```

To instantiate the FirstClass we use this statement:
```java
FirstClass f=new FirstClass();
```

f is used to refer FirstClass object

#### 11) What is encapsulation ?

The process of wrapping or putting up of data in to a single unit class and 
keeps data safe from misuse is called encapsulation .

Through encapsulation we can hide and protect the data stored in java objects.Java supports 
encapsulation through access control. There are four access control modifiers in java public , private 
,protected and default level.

For example take a car class , In car we have many parts which is not required for driver to know what all 
it consists inside. He is required to know only about how to start and stop the car. So we can expose 
what all are required and hide the rest by using encapsulation.

#### 12)What is constructor in java ?

 A constructor is a special method used to initialize objects in java.
we use constructors to initialize all variables in the class when an object is created. As and when an object 
is created it is initialized automatically with the help of constructor in java.

We have two types of constructors
Default Constructor
Parameterized Constructor

Signature : public classname()
{
}

Signature : public classname(parameters list)
{
}

#### 13) Difference between overriding and overloading in java?

Overriding Overloading

In overriding method names must be same In overloading method names must be same
Argument List must be same Argument list must be different atleast order of 
arguments.
Return type can be same or we can return covariant 
type. From 1.5 covariant types are allowed
Return type can be different in overloading.
We cant increase the level of checked exceptions. 
No restrictions for unchecked exceptions
In overloading different exceptions can be thrown.
A method can only be overridden in subclass A method can be overloaded in same class or 
subclass
Private,static and final variables cannot be 
overridden.
Private , static and final variables can be 
overloaded.
In overriding which method is called is decided at 
runtime based on the type of object referenced at 
run time
In overloading which method to call is decided at 
compile time based on reference type.
Overriding is also known as Runtime polymorphism, 
dynamic polymorphism or late binding
Overloading is also known as Compile time 
polymorphism, static polymorphism or early 
binding.

#### 14) What is ‘IS-A ‘ relationship in java?

‘is a’ relationship is also known as inheritance. We can implement ‘is a’ relationship or inheritance in java 
using extends keyword. The advantage or inheritance or is a relationship is reusability of code instead of 
duplicating the code.
Ex : Motor cycle is a vehicle
Car is a vehicle Both car and motorcycle extends vehicle.

#### 15) What is ‘HAS A’’ relationship in java?

‘Has a ‘ relationship is also known as “composition or Aggregation”. As in inheritance we have ‘extends’ 
keyword we don’t have any keyword to implement ‘Has a’ relationship in java. The main advantage of 
‘Has-A‘ relationship in java code reusability.

#### 16) Difference between ‘IS-A’ and ‘HAS-A’ relationship in java?

IS-A relationship HAS- A RELATIONSHIP
Is a relationship also known as inheritance Has a relationship also known as composition or 
aggregation.
For IS-A relationship we uses extends keyword For Has a relationship we use new keyword
Ex : Car is a vehicle. Ex : Car has an engine. We cannot say Car is an 
engine
The main advantage of inheritance is reusability of 
code
The main advantage of has a relationship is 
reusability of code.

#### 17) Explain about instanceof operator in java?

Instanceof operator is used to test the object is of which type.
Syntax : <reference expression> instanceof <destination type>
Instanceof returns true if reference expression is subtype of destination type.
Instanceof returns false if reference expression is null.
Example : 
public classInstanceOfExample {
    public static voidmain(String[] args) {
        Integer a = new Integer(5);
        if (a instanceof java.lang.Integer) {
            System.out.println(true);
        } else {
            System.out.println(false);
        }
    }
}

Since a is integer object it returns true.
There will be a compile time check whether reference expression is subtype of destination type. If it is not 
a subtype then compile time error will be shown as Incompatible types

#### 18) Can we have multiple classes in single file ? 

Yes we can have multiple classes in single file but it people rarely do that and not recommended. We can 
have multiple classes in File but only one class can be made public. If we try to make two classes in File 
public we get following compilation error.

“The public type must be defined in its own file”.

#### 19) What are packages in java? 

Package is a mechanism to group related classes ,interfaces and enums in to a single module.
Package can be declared using the following statement :
Syntax : package <package-name>
Coding Convention : package name should be declared in small letters.
package statement defines the namespace.

The main use of package is

1) To resolve naming conflicts
2) For visibility control : We can define classes and interfaces that are not accessible outside the 
class.

#### 20) Can we have more than one package statement in source file ?

We can’t have more than one package statement in source file. In any java program there can be atmost 
only 1 package statement. We will get compilation error if we have more than one package statement in 
source file.

#### 21) Can we define package statement after import statement in java?

We can’t define package statement after import statement in java. package statement must be the first 
statement in source file. We can have comments before the package statement.

#### 22) Explain about abstract classes in java?

Sometimes we may come across a situation where we cannot provide implementation to all the methods 
in a class. We want to leave the implementation to a class that extends it. In such case we declare a class 
as abstract.To make a class abstract we use key word abstract. Any class that contains one or more 
abstract methods is declared as abstract. If we don’t declare class as abstract which contains abstract 
methods we get compile time error. We get the following error.
“The type <class-name> must be an abstract class to define abstract methods.”

Signature ; abstract class <class-name>
{
}
For example if we take a vehicle class we cannot provide implementation to it because there may be two 
wheelers , four wheelers etc. At that moment we make vehicle class abstract. All the common features of 
vehicles are declared as abstract methods in vehicle class. Any class which extends vehicle will provide 
its method implementation. It’s the responsibility of subclass to provide implementation.

The important features of abstract classes are :
1) Abstract classes cannot be instantiated.
2) An abstract classes contains abstract methods, concrete methods or both.
3) Any class which extends abstract class must override all methods of abstract class.
4) An abstract class can contain either 0 or more abstract methods.

Though we cannot instantiate abstract classes we can create object references . Through superclass 
references we can point to subclass.

#### 23) Can we create constructor in abstract class ?

We can create constructor in abstract class , it does’nt give any compilation error. But when we cannot 
instantiate class there is no use in creating a constructor for abstract class.

#### 24) What are abstract methods in java?

An abstract method is the method which does’nt have any body. Abstract method is declared with 
keyword abstract and semicolon in place of method body.

Signature : public abstract void <method name>();
Ex : public abstract void getDetails();
It is the responsibility of subclass to provide implementation to abstract method defined in abstract class