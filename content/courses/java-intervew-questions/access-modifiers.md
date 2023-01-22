---
title: Access Modifiers
description: Access Modifiers
weight: 20
lastmod: 2022-11-20T10:23:30-09:00
draft: false
vimeo: 773633416
emoji: 🚆
video_length: 1:33
chapter_start: 
free: true
---


#### 1) What all access modifiers are allowed for top class ?

For top level class only two access modifiers are allowed. public and default. If a class is declared as 
public it is visible everywhere.

If a class is declared default it is visible only in same package.

If we try to give private and protected as access modifier to class we get the below compilation error.

Illegal Modifier for the class only public,abstract and final are permitted.

#### 2) What are access modifiers in java?

The important feature of encapsulation is access control. By preventing access control we can misuse of 
class, methods and members.

A class, method or variable can be accessed is determined by the access modifier. There are three types 
of access modifiers in java. public,private,protected. If no access modifier is specified then it has a default 
access.

#### 3) What access modifiers can be used for class ?

We can use only two access modifiers for class public and default.

public: A class with public modifier can be visible
1) In the same class
2) In the same package subclass
3) In the same package nonsubclass
4) In the different package subclass
5) In the different package non subclass.

default : A class with default modifier can be accesed
1) In the same class
2) In the same package subclass
3) In the same package nonsubclass
4) In the different package subclass
5) In the different package non subclass.

#### 4) Explain what access modifiers can be used for methods?

We can use all access modifiers public, private,protected and default for methods.

public : When a method is declared as public it can be accessed
1) In the same class
2) In the same package subclass
3) In the same package nonsubclass
4) In the different package subclass
5) In the different package non subclass.

default : When a method is declared as default, we can access that method in
1) In the same class
2) In the same package subclass
3) In the same package non subclass

We cannot access default access method in
1) Different package subclass
2) Different package non subclass.

protected : When a method is declared as protected it can be accessed
1) With in the same class
2) With in the same package subclass
3) With in the same package non subclass
4) With in different package subclass
It cannot be accessed non subclass in different package.

private : When a method is declared as private it can be accessed only in that class.
It cannot be accessed in
1) Same package subclass
2) Same package non subclass
3) Different package subclass
4) Different package non subclass

#### 5) Explain what access modifiers can be used for methods?

We can use all access modifiers public, private,protected and default for methods.

public : When a method is declared as public it can be accessed
1) In the same class
2) In the same package subclass
3) In the same package nonsubclass
4) In the different package subclass
5) In the different package non subclass.

default : When a method is declared as default, we can access that method in
1) In the same class
2) In the same package subclass
3) In the same package non subclass
We cannot access default access method in
1) Different package subclass
2) Different package non subclass.

protected : When a method is declared as protected it can be accessed
1) With in the same class
2) With in the same package subclass
3) With in the same package non subclass
4) With in different package subclass
It cannot be accessed non subclass in different package.

private : When a method is declared as private it can be accessed only in that class.
It cannot be accessed in
1) Same package subclass
2) Same package non subclass
3) Different package subclass
4) Different package non subclass

#### 6) What is final access modifier in java?

final access modifier can be used for class, method and variables. The main advantage of final access 
modifier is security no one can modify our classes, variables and methods. The main disadvantage of final 
access modifier is we cannot implement oops concepts in java. Ex : Inheritance, polymorphism.

final class : A final class cannot be extended or subclassed. We are preventing inheritance by marking a 
class as final. But we can still access the methods of this class by composition. Ex: String class

final methods: Method overriding is one of the important features in java. But there are situations where 
we may not want to use this feature. Then we declared method as final which will print overriding. To 
allow a method from being overridden we use final access modifier for methods.

final variables : If a variable is declared as final ,it behaves like a constant . We cannot modify the value 
of final variable. Any attempt to modify the final variable results in compilation error. The error is as 
follows
“final variable cannot be assigned.”

