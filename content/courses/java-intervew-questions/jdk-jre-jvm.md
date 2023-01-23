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

#### 5) What is the Java compilation process?
The Java compilation process is the process of converting a Java source code file (.java) into a bytecode file (.class) that can be executed by the Java Virtual Machine (JVM). The compilation is done using the Java compiler (javac) which is a part of the Java Development Kit (JDK).

#### 6) What is the Java Virtual Machine (JVM)?
The Java Virtual Machine (JVM) is a software that interprets and executes Java bytecode. It provides a platform-independent environment for running Java programs, regardless of the underlying operating system or hardware.

#### 7) What is the difference between JVM, JRE, and JDK?
JVM (Java Virtual Machine) is a virtual machine that interprets and executes Java bytecode.
JRE (Java Runtime Environment) is a package that includes the JVM and the Java Standard Library, which provides the necessary resources to run Java programs.
JDK (Java Development Kit) is a package that includes the JRE, the Java compiler (javac), and other development tools needed for creating and compiling Java programs.

#### 8) What are the different components of JVM?
The different components of JVM are: ClassLoader, Heap, Stack, PC Register, Native Method Stack, Execution Engine and Method Area.

#### 9) What is the role of classloader in JVM?
The classloader is responsible for loading class files into the JVM. It loads the required classes, verifies their integrity, and creates an instance of java.lang.Class for each class.

#### 10) What is the role of heap in JVM?
The heap is the memory space where the JVM stores all the objects created at runtime. It is responsible for allocating memory for new objects and for garbage collection.

#### 11) What is the role of stack in JVM?
The stack is the memory space where the JVM stores the state of each thread. It stores the method calls, local variables, and the return value of each method call.

#### 12) What is the role of PC register in JVM?
The PC (Program Counter) register is used by the JVM to keep track of the next instruction to be executed by the current thread.

#### 13) What is the role of native method stack in JVM?
The native method stack is used by the JVM to store the state of native methods, which are written in a language other than Java and are used in the program.

#### 14) What is the role of execution engine in JVM?

The execution engine is responsible for interpreting and executing the Java bytecode. It reads the bytecode instructions and performs the corresponding actions, such as allocating memory, performing calculations, and making method calls.

#### 15) What is the role of method area in JVM?
The method area is a memory space where the JVM stores the information about class and method level structure of a program. It stores the class level structure, method level structure and constant pool of the class.

#### 16) What is the role of JIT (Just-in-Time) compiler in JVM?
JIT (Just-in-Time) compiler is a component of JVM that dynamically compiles the bytecode into native machine code at runtime. This improves the performance of the program by reducing the overhead of interpreting the bytecode.

#### 17) What is the role of Garbage Collection in JVM?
Garbage Collection is a process that automatically frees up memory used by objects that are no longer needed. It is responsible for reclaiming the heap memory by removing unreferenced objects and making the memory available for new objects.

#### 18) How does JVM handle the exception?
JVM uses a technique called "exception handling" to handle exceptions. When an exception occurs, JVM checks the exception against the exception handlers in the method that throws the exception. If a matching handler is found, the exception is handed off to that handler. If no matching handler is found, the exception is propagated up the call stack until a matching handler is found.

#### 19) What is the role of classpath in JVM?
Classpath is a parameter that the JVM uses to locate and load classes at runtime. The classpath is a list of directories and jar files that the JVM looks in to find the classes it needs to execute a program.
