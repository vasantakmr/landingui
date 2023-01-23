---
title: String Handling
description: strings
weight: 12
lastmod: 2022-11-20T10:23:30-09:00
draft: false
vimeo: 773632607
emoji: 🎭
video_length: 2:56
quiz: true
free: true
---

<quiz-modal options="96:97:98:99" answer="98" prize="5">
  <h6>What is 'b' ASCII Code?</h6>
</quiz-modal>

#### 1) What is ASCII Code?

ASCII stands for American Standard code for Information Interchange. ASCII character range is 0 to 255. 
We can’t add more characters to the ASCII Character set. ASCII character set supports only English. That 
13
is the reason, if we see C language we can write c language only in English we can’t write in other 
languages because it uses ASCII code.

#### 2) What is Unicode ?

Unicode is a character set developed by Unicode Consortium. To support all languages in the world Java 
supports Unicode values. Unicode characters were represented by 16 bits and its character range is 0-
65,535.
Java uses ASCII code for all input elements except for Strings,identifiers, and comments. If we want to 
use telugu we can use telugu characters for identifiers.We can enter comments in telugu.

#### 3) Difference between Character Constant and String Constant in java ?

Character constant is enclosed in single quotes. String constants are enclosed in double quotes. Character 
constants are single digit or character. String Constants are collection of characters.

Ex :’2’, ‘A’
Ex : “Hello World”

#### 4) What are constants and how to create constants in java?

Constants are fixed values whose values cannot be changed during the execution of program. We create 
constants in java using final keyword.

Ex : final int number =10;
final String str=”java-interview –questions”


#### 5) What is a string in Java?
A string in Java is a sequence of characters. It is an object of the String class, which is immutable and can store any combination of characters.

#### 6) How do you declare a string variable in Java?
To declare a string variable in Java, you use the String data type and the variable name. Example:

String myString;

#### 7) How do you initialize a string variable in Java?
To initialize a string variable in Java, you can use the assignment operator = and assign a string of characters to the variable. Example:

String myString = "Hello World!";

#### 8) How do you concatenate strings in Java?
To concatenate strings in Java, you can use the + operator. Example:

String myString = "Hello" + " " + "World!";

#### 9) How do you compare strings in Java?
To compare strings in Java, you can use the equals() method or the == operator. The equals() method compares the characters of the strings while the == operator compares the memory locations of the strings.

#### 10) How do you find the length of a string in Java?
To find the length of a string in Java, you can use the length() method. Example:

int length = myString.length();

#### 11) How do you extract a substring from a string in Java?
- To extract a substring from a string in Java, you can use the `substring()` method. The method takes two parameters, the starting index and the ending index of the substring. Example:
String mySubstring = myString.substring(6, 11);

#### 12) How do you check if a string contains a specific word or substring in Java?
- To check if a string contains a specific word or substring in Java, you can use the `contains()` method. This method returns a boolean value indicating whether the specified substring is present in the string or not. Example:
boolean contains = myString.contains("World");

#### 13) How do you replace a specific word or substring in a string in Java?
- To replace a specific word or substring in a string in Java, you can use the `replace()` method. This method takes two parameters, the substring to be replaced and the replacement substring. Example:
String newString = myString.replace("World", "Java");

#### 14) How do you convert a string to an array of characters in Java?
- To convert a string to an array of characters in Java, you can use the `toCharArray()` method. This method returns a character array of the string. Example:
char[] myCharArray = myString.toCharArray();

#### 15) How do you split a string into an array of substrings in Java?
- To split a string into an array of substrings in Java, you can use the `split()` method. This method takes a regular expression as a parameter and returns an array of substrings split by the specified regular expression. Example:
String[] myStringArray = myString.split(" ");

#### 16) How do you convert a string to uppercase or lowercase in Java?
- To convert a string to uppercase or lowercase in Java, you can use the `toUpperCase()` or `toLowerCase()` method respectively. Example:
String upperString = myString.toUpperCase();
String lowerString = myString.toLowerCase();

#### 17) How do you trim leading and trailing whitespaces from a string in Java?
- To trim leading and trailing whitespaces from a string in Java, you can use the `trim()` method. This method returns a new string with the leading and trailing whitespaces removed. Example:
String myTrimmedString = myString.trim();

#### 18) How do you check if a string starts or ends with a specific word or substring in Java?
- To check if a string starts or ends with a specific word or substring in Java, you can use the `startsWith()` or `endsWith()` method respectively. These methods take a substring as a parameter and return a boolean value indicating whether the string starts or ends with the specified substring. Example:
boolean startsWith = myString.startsWith("Hello");
boolean endsWith = myString.endsWith("!");


#### 19) How do you use the `StringBuilder` class to create a mutable strng?

To use the StringBuilder class to create a mutable string, you can use its constructor to create a new instance of the class. The StringBuilder class has many methods similar to the String class, such as append(), insert(), delete(), reverse(), etc. Example:

StringBuilder myStringBuilder = new StringBuilder("Hello ");
myStringBuilder.append("World");

#### 20) How do you use the StringBuffer class to create a thread-safe mutable string in Java?
To use the StringBuffer class to create a thread-safe mutable string in Java, you can use its constructor to create a new instance of the class. The StringBuffer class has the same methods as the StringBuilder class and it is thread-safe, which means that it can be used in a multithreaded environment without any additional synchronization. Example:

StringBuffer myStringBuffer = new StringBuffer("Hello ");
myStringBuffer.append("World");

#### 21) How do you use the format() method to format a string in Java?
To use the format() method to format a string in Java, you can pass in a format string and a set of arguments that will be filled in placeholders in the format string. Example:

String myFormattedString = String.format("Hello, %s!", "World");

#### 22) How do you use the printf() method to format a string in Java?
To use the printf() method to format a string in Java, you can pass in a format string and a set of arguments that will be filled in placeholders in the format string. This method is typically used to print the formatted string to the console. Example:

System.out.printf("Hello, %s!", "World");

#### 23) How do you use the join() method to join an array of strings into a single string in Java?
To use the join() method to join an array of strings into a single string in Java, you can pass in a delimiter and an array of strings. This method returns a new string that is the concatenation of the strings in the array, separated by the delimiter. Example:

String myJoinedString = String.join(", ", myStringArray);

#### 24) How do you use the replaceAll() method to replace all occurences of a word or substring in a string in Java?
To use the replaceAll() method to replace all occurences of a word or substring in a string in Java, you can pass in a regular expression and a replacement string. This method returns a new string with all occurences of the regular expression replaced by the replacement string.

Example:

String myReplacedString = myString.replaceAll("[aeiou]", "*");

This will replace all vowels in myString with the * character.



