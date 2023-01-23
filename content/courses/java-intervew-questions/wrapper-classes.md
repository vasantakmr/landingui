---
title: Wrapper Classes
description: Wrapper Classes
weight: 23
lastmod: 2022-11-20T10:23:30-09:00
draft: false
vimeo: 773628343
emoji: 👮‍♂️
video_length: 1:25
free: true
---

#### 1) What are wrapper classes in Java?
Wrapper classes in Java are classes that wrap primitive data types. They provide an object-oriented way to work with primitive data types. Each primitive data type has a corresponding wrapper class.

#### 2) What are the different wrapper classes in Java?
The different wrapper classes in Java are: Integer for int, Long for long, Short for short, Byte for byte, Float for float, Double for double, Boolean for boolean, and Character for char.

#### 3) How do you create an object of a wrapper class in Java?
To create an object of a wrapper class in Java, you can use the constructor of the class and pass in the primitive value. Example:
```java
Integer myInt = new Integer(10);
```

#### 4) How do you convert a primitive data type to a wrapper class object in Java?
To convert a primitive data type to a wrapper class object in Java, you can use the valueOf() method of the corresponding wrapper class. Example:
```java
Integer myInt = Integer.valueOf(10);
```

#### 5) How do you convert a wrapper class object to a primitive data type in Java?
To convert a wrapper class object to a primitive data type in Java, you can use the xxxValue() method of the wrapper class, where xxx is the name of the primitive data type. Example:
```java
int myPrimitive = myInt.intValue();
```

#### 6) How do you convert a string to a wrapper class object in Java?
To convert a string to a wrapper class object in Java, you can use the parseXxx() method of the corresponding wrapper class, where Xxx is the name of the primitive data type. Example:
```java
Integer myInt = Integer.parseInt("10");
```

#### 7) How do you compare wrapper class objects in Java?
To compare wrapper class objects in Java, you can use the compareTo() method. This method returns a negative integer, zero, or a positive integer, depending on whether the first object is less than, equal to, or greater than the second object. Example:
```java
int result = myInt1.compareTo(myInt2);
```

#### 8) How do you use the MAX_VALUE and MIN_VALUE constants of a wrapper class in Java?
To use the MAX_VALUE and MIN_VALUE constants of a wrapper class in Java, you can access the constants directly from the class. These constants represent the maximum and minimum values that the corresponding primitive data type can hold. Example:

```java
int maxInt = Integer.MAX_VALUE;
int minInt = Integer.MIN_VALUE;
```

#### 9) How do you use the toString() method of a wrapper class in Java?
To use the toString() method of a wrapper class in Java, you can call the method on an instance of the wrapper class. This method returns a string representation of the object's value. Example:
```java
String myIntString = myInt.toString();
```
#### 10) How do you use the valueOf() method of a wrapper class in Java?
To use the valueOf() method of a wrapper class in Java, you can call the method on the class and pass in a string representation of the value. This method returns an object of the corresponding wrapper class. Example:
```java
Integer myInt = Integer.valueOf("10");
```

#### 11) How do you use the parseXxx() method of a wrapper class in Java?
To use the parseXxx() method of a wrapper class in Java, you can call the method on the class and pass in a string representation of the value. This method returns the primitive data type value. Example:
```java
int myPrimitive = Integer.parseInt("10");
```

#### 12) How do you use the toXxxString() method of a wrapper class in Java?
To use the toXxxString() method of a wrapper class in Java, you can call the method on an instance of the wrapper class. This method returns a string representation of the object's value in the corresponding primitive data type. Example:
```java
String myIntHexString = Integer.toHexString(255);
```

#### 13) How do you use the sum(), min(), and max() static methods of a wrapper class in Java?
To use the sum(), min(), and max() static methods of a wrapper class in Java, you can call the method on the class and pass in two objects of the corresponding wrapper class. These methods return the sum, minimum, or maximum value of the two objects. Example:
```java
Integer sum = Integer.sum(10, 20);
Integer min = Integer.min(10, 20);
Integer max = Integer.max(10, 20);
```

#### 14) How do you use the compare() static method of a wrapper class in Java?
To use the compare() static method of a wrapper class in Java, you can call the method on the class and pass in two objects of the corresponding wrapper class. This method returns an int value of -1, 0, or 1 indicating whether the first argument is less than, equal to, or greater than the second argument. Example:
```java
int compare = Integer.compare(10, 20);
```

#### 15) How do you use the decode() method of a wrapper class in Java?
To use the decode() method of a wrapper class in Java, you can call the method on the class and pass in a string representation of the value. This method returns an object of the corresponding wrapper class after parsing the input string as a number in the specified radix. The radix can be specified in the format of 0x for hexadecimal, 0 for octal, or # for decimal. Example:

```java
Integer myInt = Integer.decode("0xFF"); //255 in decimal
```
