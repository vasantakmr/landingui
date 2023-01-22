---
title: JDK JRE JVM
description: How JVM, JRE and JDK works
weight: 1
lastmod: 2022-11-20T10:23:30-09:00
draft: false
vimeo: 773633635
emoji: 🚆
video_length: 1:33
free: true 
---

#### 1) Why java is platform independent?

The most unique feature of java is platform independent. In any programming language soruce code is 
compiled in to executable code . This cannot be run across all platforms. When javac compiles a java 
program it generates an executable file called .class file.

class file contains byte codes. Byte codes are interpreted only by JVM’s . Since these JVM’s are made 
available across all platforms by Sun Microsystems, we can execute this byte code in any platform. Byte 
code generated in windows environment can also be executed in linux environment. This makes java 
platform independent.

#### 2) What is JIT compiler ?

JIT compiler stands for Just in time compiler. JIT compiler compiles byte code in to executable code . 
JIT a part of JVM .JIT cannot convert complete java program in to executable code it converts as and 
when it is needed during execution.

#### 3) What is bytecode in java ?

When a javac compiler compiler compiles a class it generates .class file. This .class file contains set of 
instructions called byte code. Byte code is a machine independent language and contains set of 
instructions which are to be executed only by JVM. JVM can understand this byte codes.

#### 4) What is difference between c++ and Java ?

| Java  | C++  |
|---|---|
| 1) Java is platform independent | 1)  C++ is platform dependent. |
| 2) There are no pointers in java   | 2) There are pointers in C++. |
| 3) There is no operator overloading in java  | 3) C ++ has operator overloading.  |
| 4) There is garbage collection in java   | 4) There is no garbage collection  |
| 5) Supports multithreading  |  5) Does’nt support multithreading |
| 6) There are no templates in java  |  6) There are templates in java |
| 7) There are no global variables in java   | 7) There are global variables in c++  |

