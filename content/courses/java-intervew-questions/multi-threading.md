---
title: Multi Threading
description: Multi Threading
weight: 22
lastmod: 2022-11-20T10:23:30-09:00
draft: false
vimeo: 773633923
emoji: 👋
chapter_start: 
video_length: 1:33
free: true 
---

#### 1) What is process ?

A process is a program in execution.
Every process have their own memory space.Process are heavy weight and requires their own address 
space. One or more threads make a process.

#### 2) What is thread in java?

Thread is separate path of execution in program.
Threads are
1) Light weight
2) They share the same address space.
3) Creating thread is simple when compared to process because creating thread requires less resources 
when compared to process
4) Threads exists in process. A process have atleast one thread.

#### 3) Difference between process and thread?

 Process Thread
1) Program in execution. Separate path of execution in program. One or 
more threads is called as process.
2) Processes are heavy weight Threads are light weight.
3) Processes require separate address space. Threads share same address space.
4) Interprocess communication is expensive. Interthread communication is less expensive 
compared to processes.
5) Context switching from one process to another 
is costly.
Context switching between threads is low cost.

#### 4) What is multitasking ?

Multitasking means performing more than one activity at a time on the computer. Example Using 
spreadsheet and using calculator at same time.

#### 5) What are different types of multitasking?

There are two different types of multitasking :

1) Process based multitasking
2) Thread based multitasking
Process based multitasking : It allows to run two or more programs concurrently. In process 
based multitasking a process is the smallest part of code .
Example : Running Ms word and Ms powerpoint at a time.
Thread based multitasking : It allows to run parts of a program to run concurrently.
Example : Formatting the text and printing word document at same time .
Java supports thread based multitasking and provides built in support for multithreading.

#### 6) What are the benefits of multithreaded programming?

Multithreading enables to use idle time of cpu to another thread which results in faster execution of 
program. In single threaded environment each task has to be completed before proceeding to next task
making cpu idle.

#### 7) Explain thread in java?

1) Thread is independent path of execution with in a program.
2) A thread consists of three parts Virtual Cpu, Code and data.
3) At run time threads share code and data i.e they use same address space.
4) Every thread in java is an object of java.lang.Thread class.

#### 8) List Java API that supports threads?
java.lang.Thread : This is one of the way to create a thread. By extending Thread class and overriding 
run() we can create thread in java.

java.lang.Runnable : Runnable is an interface in java. By implementing runnable interface and overriding 
run() we can create thread in java.

java.lang.Object : Object class is the super class for all the classes in java. In object class we have three 
methods wait(), notify(), notifyAll() that supports threads.

java.util.concurrent : This package has classes and interfaces that supports concurrent programming.
Ex : Executor interface, Future task class etc.

#### 9) Explain about main thread in java?

Main thread is the first thread that starts immediately after a program is started.
Main thread is important because :
1) All the child threads spawn from main thread.
2) Main method is the last thread to finish execution.
When JVM calls main method() it starts a new thread. Main() method is temporarily stopped while the 
new thread starts running.

#### 10) In how many ways we can create threads in java?

We can create threads in java by any of the two ways :
1) By extending Thread class
2) By Implementing Runnable interface.